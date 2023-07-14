# Comparing `tmp/waveformtools-2023.6.5.tar.gz` & `tmp/waveformtools-2023.7.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waveformtools-2023.6.5.tar", last modified: Mon Jun  5 10:03:38 2023, max compression
+gzip compressed data, was "waveformtools-2023.7.14.tar", last modified: Fri Jul 14 16:00:54 2023, max compression
```

## Comparing `waveformtools-2023.6.5.tar` & `waveformtools-2023.7.14.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:03:38.526371 waveformtools-2023.6.5/
--rwxrwxrwx   0 root         (0) root         (0)     1075 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8758 2023-06-05 10:03:38.526371 waveformtools-2023.6.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      106 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/README
--rwxrwxrwx   0 root         (0) root         (0)     8103 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 10:03:38.526371 waveformtools-2023.6.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1396 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:03:38.524371 waveformtools-2023.6.5/waveformtools/
--rw-rw-rw-   0 root         (0) root         (0)     5480 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/BMS.py
--rw-rw-rw-   0 root         (0) root         (0)     9130 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/CoM.py
--rwxrwxrwx   0 root         (0) root         (0)     1284 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10895 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/compare.py
--rw-rw-rw-   0 root         (0) root         (0)    44315 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/dataIO.py
--rw-rw-rw-   0 root         (0) root         (0)     1698 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/diagnostics.py
--rw-rw-rw-   0 root         (0) root         (0)    27085 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/differentiate.py
--rw-rw-rw-   0 root         (0) root         (0)     9322 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/extrapolate.py
--rw-rw-rw-   0 root         (0) root         (0)    14069 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/grids.py
--rw-rw-rw-   0 root         (0) root         (0)    10952 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/integrate.py
--rw-rw-rw-   0 root         (0) root         (0)    28886 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/legacy.py
--rw-rw-rw-   0 root         (0) root         (0)    54027 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/simulations.py
--rw-rw-rw-   0 root         (0) root         (0)     6476 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/spherical.py
--rw-rw-rw-   0 root         (0) root         (0)    12506 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/transforms.py
--rw-rw-rw-   0 root         (0) root         (0)    56079 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/waveforms.py
--rw-rw-rw-   0 root         (0) root         (0)    91151 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/waveformtools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:03:38.525371 waveformtools-2023.6.5/waveformtools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8758 2023-06-05 10:03:38.000000 waveformtools-2023.6.5/waveformtools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-05 10:03:38.000000 waveformtools-2023.6.5/waveformtools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 10:03:38.000000 waveformtools-2023.6.5/waveformtools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-05 10:03:38.000000 waveformtools-2023.6.5/waveformtools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-05 10:03:38.000000 waveformtools-2023.6.5/waveformtools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 16:00:54.905798 waveformtools-2023.7.14/
+-rwxrwxrwx   0 root         (0) root         (0)     1075 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8737 2023-07-14 16:00:54.905798 waveformtools-2023.7.14/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      106 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/README
+-rwxrwxrwx   0 root         (0) root         (0)     8081 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 16:00:54.905798 waveformtools-2023.7.14/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1396 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 16:00:54.904798 waveformtools-2023.7.14/waveformtools/
+-rw-rw-rw-   0 root         (0) root         (0)     5524 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/waveformtools/BMS.py
+-rw-rw-rw-   0 root         (0) root         (0)     9282 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/waveformtools/CoM.py
+-rwxrwxrwx   0 root         (0) root         (0)     1306 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/waveformtools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11681 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/waveformtools/compare.py
+-rw-rw-rw-   0 root         (0) root         (0)    57888 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/waveformtools/dataIO.py
+-rw-rw-rw-   0 root         (0) root         (0)     1712 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/waveformtools/diagnostics.py
+-rw-rw-rw-   0 root         (0) root         (0)    27385 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/waveformtools/differentiate.py
+-rw-rw-rw-   0 root         (0) root         (0)     9599 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/waveformtools/extrapolate.py
+-rw-rw-rw-   0 root         (0) root         (0)    13697 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/waveformtools/grids.py
+-rw-rw-rw-   0 root         (0) root         (0)    11118 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/waveformtools/integrate.py
+-rw-rw-rw-   0 root         (0) root         (0)    30077 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/waveformtools/legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)    57654 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/waveformtools/simulations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6616 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/waveformtools/spherical.py
+-rw-rw-rw-   0 root         (0) root         (0)    12964 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/waveformtools/transforms.py
+-rw-rw-rw-   0 root         (0) root         (0)    92232 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/waveformtools/waveforms.py
+-rw-rw-rw-   0 root         (0) root         (0)    94038 2023-07-14 16:00:12.000000 waveformtools-2023.7.14/waveformtools/waveformtools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 16:00:54.905798 waveformtools-2023.7.14/waveformtools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8737 2023-07-14 16:00:54.000000 waveformtools-2023.7.14/waveformtools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      654 2023-07-14 16:00:54.000000 waveformtools-2023.7.14/waveformtools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 16:00:54.000000 waveformtools-2023.7.14/waveformtools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-14 16:00:54.000000 waveformtools-2023.7.14/waveformtools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-14 16:00:54.000000 waveformtools-2023.7.14/waveformtools.egg-info/top_level.txt
```

### Comparing `waveformtools-2023.6.5/LICENSE` & `waveformtools-2023.7.14/LICENSE`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.6.5/PKG-INFO` & `waveformtools-2023.7.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveformtools
-Version: 2023.6.5
+Version: 2023.7.14
 Summary:  Tools for working with numerical relativity and waveforms data 
 Home-page: https://gitlab.com/vaishakp/waveformtools
 Author: Vaishak Prasad
 Author-email: Vaishak Prasad <vaishakprasad@gmail.com>
 Project-URL: Homepage, https://gitlab.com/vaishakp/waveformtools
 Project-URL: Bug Tracker, https://gitlab.com/vaishakp/waveformtools/issues
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 License-File: LICENSE
 
 [[Project landing page]](https://sites.google.com/view/waveformtools/home)
 [![pipeline status](https://gitlab.com/vaishakp/waveformtools/badges/main/pipeline.svg)](https://gitlab.com/vaishakp/waveformtools/commits/main)
 [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://gitlab.com/vaishakp/waveformtools/commits/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/waveformtools/badge/?version=latest)](https://waveformtools.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![PyPI version](https://badge.fury.io/py/waveformtools.svg)](https://badge.fury.io/py/waveformtools)
+[![PyPI version](docs/vers_badge.svg)](https://pypi.org/project/waveformtools/)
 # Waveformtools 
 
 
 This is a python module for the handling and analysis of waveforms and data from Numerical Relativity codes, and for carrying out gravitational wave data analysis.  
 
 waveformtools is a numerical relativity data handling package that was written to aid the handling and analysis of numerical relativity data.
```

### Comparing `waveformtools-2023.6.5/README.md` & `waveformtools-2023.7.14/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [[Project landing page]](https://sites.google.com/view/waveformtools/home)
 [![pipeline status](https://gitlab.com/vaishakp/waveformtools/badges/main/pipeline.svg)](https://gitlab.com/vaishakp/waveformtools/commits/main)
 [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://gitlab.com/vaishakp/waveformtools/commits/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/waveformtools/badge/?version=latest)](https://waveformtools.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![PyPI version](https://badge.fury.io/py/waveformtools.svg)](https://badge.fury.io/py/waveformtools)
+[![PyPI version](docs/vers_badge.svg)](https://pypi.org/project/waveformtools/)
 # Waveformtools 
 
 
 This is a python module for the handling and analysis of waveforms and data from Numerical Relativity codes, and for carrying out gravitational wave data analysis.  
 
 waveformtools is a numerical relativity data handling package that was written to aid the handling and analysis of numerical relativity data.
```

### Comparing `waveformtools-2023.6.5/pyproject.toml` & `waveformtools-2023.7.14/pyproject.toml`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.6.5/setup.py` & `waveformtools-2023.7.14/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # requiremnts directly from toml
 # mreq, oreq = get_requirements()
 
 
 
 setuptools.setup(
     name="waveformtools",
- 	version="2023.06.05",
+ 	version="2023.07.14",
     author="Vaishak Prasad",
     author_email="vaishakprasad@gmail.com",
     description="Functions for handling waveform and numerical relativity data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/vaishakp/waveformtools",
     packages=setuptools.find_packages(),
```

### Comparing `waveformtools-2023.6.5/waveformtools/BMS.py` & `waveformtools-2023.7.14/waveformtools/BMS.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,17 @@
 
     # unpack the velocity vector
     vel_x, vel_y, vel_z = vec_v
 
     # magnitude of velocity
     mag_v = np.sqrt(vel_x**2 + vel_y**2 + vel_z**2)
     # compute the dot product
-    v_dot_r = np.sin(theta) * (vel_x * np.cos(phi) + vel_y * np.sin(phi)) + vel_z * np.cos(theta)
+    v_dot_r = np.sin(theta) * (
+        vel_x * np.cos(phi) + vel_y * np.sin(phi)
+    ) + vel_z * np.cos(theta)
 
     # Lorentz factor
     gamma = 1.0 / np.sqrt(1 - mag_v**2)
 
     # spin_phase
     spin_factor = np.exp(-2 * 1j * spin_phase)
 
@@ -106,15 +108,17 @@
     theta = np.pi / 2
     phi = 0.0
     for item in keys_list:
         ell = int(item[1])
         for m_index in range(2 * ell + 1):
             emm = m_index - ell
             message("ell is", ell, type(ell), "emm is ", emm)
-            supertransl_alpha_sphere += supertransl_alpha_modes[item][m_index] * Yslm(spin_weight, ell, emm, theta, phi)
+            supertransl_alpha_sphere += supertransl_alpha_modes[item][
+                m_index
+            ] * Yslm(spin_weight, ell, emm, theta, phi)
 
     return supertransl_alpha_sphere
 
 
 def boost_waveform(unboosted_waveform, conformal_factor):
     """Boost the waveform given the unboosted waveform and the boost conformal factor.
```

### Comparing `waveformtools-2023.6.5/waveformtools/CoM.py` & `waveformtools-2023.7.14/waveformtools/CoM.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,29 @@
     duration_t = time_f - time_i
     # Split the data
     x_all, y_all, z_all = Xcom
 
     # Interpolate
     from scipy.interpolate import interp1d
 
-    x_all_int_fun = interp1d(time_axis, np.power(time_axis, order) * x_all / duration_t, kind="quadratic")
-    y_all_int_fun = interp1d(time_axis, np.power(time_axis, order) * y_all / duration_t, kind="quadratic")
-    z_all_int_fun = interp1d(time_axis, np.power(time_axis, order) * z_all / duration_t, kind="quadratic")
+    x_all_int_fun = interp1d(
+        time_axis,
+        np.power(time_axis, order) * x_all / duration_t,
+        kind="quadratic",
+    )
+    y_all_int_fun = interp1d(
+        time_axis,
+        np.power(time_axis, order) * y_all / duration_t,
+        kind="quadratic",
+    )
+    z_all_int_fun = interp1d(
+        time_axis,
+        np.power(time_axis, order) * z_all / duration_t,
+        kind="quadratic",
+    )
 
     int_funcs = [x_all_int_fun, y_all_int_fun, z_all_int_fun]
 
     # Integrate
     from scipy.integrate import quad
 
     moments = {}
@@ -83,15 +95,16 @@
 
     com_alpha:		list
                                     The list containig the alpha parameter vector
 
     """
 
     com_alpha = (
-        4 * (time_f**2 + time_f * time_i + time_i**2) * np.array(Xcom_0) - 6 * (time_f + time_i) * np.array(Xcom_1)
+        4 * (time_f**2 + time_f * time_i + time_i**2) * np.array(Xcom_0)
+        - 6 * (time_f + time_i) * np.array(Xcom_1)
     ) / (time_f - time_i) ** 2
 
     return com_alpha
 
 
 def compute_com_beta(time_i, time_f, Xcom_0, Xcom_1):
     """Computes the CoM beta parameter: the mean drift of the system,
@@ -113,15 +126,17 @@
     -------
 
     com_beta:		list
                             The list containig the alpha parameter vector
 
     """
 
-    com_beta = (12 * (Xcom_1) - 6 * (time_f + time_i) * Xcom_0) / (time_f - time_i) ** 2
+    com_beta = (12 * (Xcom_1) - 6 * (time_f + time_i) * Xcom_0) / (
+        time_f - time_i
+    ) ** 2
 
     return com_beta
 
 
 def compute_conformal_k(vec_v, info, spin_phase=0):
     """Compute the conformal factor for the boost transformation
             :math:`k = \\exp(-2i \\lambda) \\gamma^3 (1 - \\mathbf{v} \\cdot \\mathbf{r})^3
@@ -158,15 +173,17 @@
     # magnitude of velocity
     mag_v = np.sqrt(vel_x**2 + vel_y**2 + vel_z**2)
 
     # Compute the 2d co-ordinate axis on the sphere
     theta, phi = info.meshgrid
 
     # compute the dot product
-    v_dot_r = np.sin(theta) * (vel_x * np.cos(phi) + vel_y * np.sin(phi)) + vel_z * np.cos(theta)
+    v_dot_r = np.sin(theta) * (
+        vel_x * np.cos(phi) + vel_y * np.sin(phi)
+    ) + vel_z * np.cos(theta)
 
     # Lorentz factor
     gamma = 1.0 / np.sqrt(1 - mag_v**2)
 
     # spin_phase
     spin_factor = np.exp(-2 * 1j * spin_phase)
 
@@ -280,11 +297,14 @@
 
         # conformal_k_on_sphere = compute_conformal_k(vec_v, theta, phi)
         boosted_waveform_item = conformal_factor * item
 
         boosted_waveform_data.append(boosted_waveform_item)
 
     # Construct a 2d waveform array object
-    boosted_waveform = spherical_array(gridinfo=unboosted_waveform.gridinfo, data=np.array(boosted_waveform_data))
+    boosted_waveform = spherical_array(
+        gridinfo=unboosted_waveform.gridinfo,
+        data=np.array(boosted_waveform_data),
+    )
     boosted_waveform.label = "boosted"
 
     return boosted_waveform
```

### Comparing `waveformtools-2023.6.5/waveformtools/__init__.py` & `waveformtools-2023.7.14/waveformtools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     # print(package_directory)
     # Open the file
     vers = "-1"
     try:
         with open(package_directory + "/../public/version", "r") as vers_file:
             vers = vers_file.readlines()[0]
     except Exception as excep:
-        print("This is not a git repo! please use the version attribute instead!")
+        print(
+            "This is not a git repo! please use the version attribute instead!"
+        )
     # with open(package_directory + "/../public/date.txt", "r") as vers_file:
     # vers = vers_file.read()[:10]
 
     return vers
 
 
-__version__ = "2023.06.05"
+__version__ = "2023.07.14"
```

### Comparing `waveformtools-2023.6.5/waveformtools/compare.py` & `waveformtools-2023.7.14/waveformtools/compare.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,23 @@
 # plt.rcParams.update({"axes.labelweight" : "bold"})
 plt.rcParams.update({"font.style": "normal"})
 plt.rcParams.update({"legend.markerscale": 9})
 
 # from waveformtools.waveforms import modes_array
 
 
-def plot_modes(wf1, nmodes=3, save_fig=False, xlim=[-1200, 100], ylim="auto", nstop=1, plot22=False):
+def plot_modes(
+    wf1,
+    nmodes=3,
+    save_fig=False,
+    xlim=[-1200, 100],
+    ylim="auto",
+    nstop=1,
+    plot22=False,
+):
     """Plot the first `nmodes` dominant modes of
     the input waveforms
 
     Parameters
     ----------
     wf:           modes_array
                               The list of `modes_array` waveforms
@@ -97,28 +105,50 @@
         for emm in emm_list:
             mode_values = wf1.mode(ell, emm)
             mode_amp = np.absolute(mode_values)
             max_mode_value = np.amax(mode_values)
 
             mode_phase = xtract_cphase(mode_values.real, mode_values.imag)
 
-            ax1.scatter(wf1.time_axis[:], mode_amp[:], label=rf"$\ell${ell}$m${emm}", s=1, alpha=0.2 * abs(emm) % 1)
-            ax2.scatter(wf1.time_axis[:], abs(mode_phase[:]), label=rf"$\ell${ell}$m${emm}", s=1)
+            ax1.scatter(
+                wf1.time_axis[:],
+                mode_amp[:],
+                label=rf"$\ell${ell}$m${emm}",
+                s=1,
+                alpha=0.2 * abs(emm) % 1,
+            )
+            ax2.scatter(
+                wf1.time_axis[:],
+                abs(mode_phase[:]),
+                label=rf"$\ell${ell}$m${emm}",
+                s=1,
+            )
 
     if plot22:
         ell = 2
         emm = 2
         mode_values = wf1.mode(ell, emm)
         mode_amp = np.absolute(mode_values)
         max_mode_value = np.amax(mode_values)
 
         mode_phase = xtract_cphase(mode_values.real, mode_values.imag)
 
-        ax1.scatter(wf1.time_axis[:], mode_amp[:], label=rf"$\ell${ell}$m${emm}", s=1, alpha=0.2 * abs(emm) % 1)
-        ax2.scatter(wf1.time_axis[:], abs(mode_phase[:]), label=rf"$\ell${ell}$m${emm}", s=1)
+        ax1.scatter(
+            wf1.time_axis[:],
+            mode_amp[:],
+            label=rf"$\ell${ell}$m${emm}",
+            s=1,
+            alpha=0.2 * abs(emm) % 1,
+        )
+        ax2.scatter(
+            wf1.time_axis[:],
+            abs(mode_phase[:]),
+            label=rf"$\ell${ell}$m${emm}",
+            s=1,
+        )
 
     ax1.grid(which="both")
     ax2.grid(which="both")
     ax1.legend()
     ax2.legend()
     plt.tight_layout()
     ax1.set_xlabel("t/M")
@@ -143,15 +173,21 @@
         fig1.savefig(f"{wf1.label}_waveform_amp_modes.pdf")
         fig2.savefig(f"{wf1.label}_waveform_phase_modes.pdf")
 
     plt.show()
 
 
 def plot_mode_differences(
-    waveforms, nmodes=3, save_fig=False, xlabel="t/M", ylabel=r"r\Psi_{4}^{(\ell m)}", labels=None, xlim=[-1000, 100]
+    waveforms,
+    nmodes=3,
+    save_fig=False,
+    xlabel="t/M",
+    ylabel=r"r\Psi_{4}^{(\ell m)}",
+    labels=None,
+    xlim=[-1000, 100],
 ):
     """Plot the fractional difference of the first `nmodes`
     dominant modes of the input waveforms.
 
     Parameters
     ----------
     waveforms:    modes_array
@@ -270,15 +306,17 @@
             mode_phase_resam0 = mode_phase_int_fun0(new_time_axis)
 
             for index, wfx in enumerate(waveforms[1:]):
                 label = wfx.label  # labels[index+1]
 
                 mode_valuesx = wfx.mode(ell, emm)
                 mode_ampx = np.absolute(mode_valuesx)
-                mode_phasex = xtract_cphase(mode_valuesx.real, mode_valuesx.imag)
+                mode_phasex = xtract_cphase(
+                    mode_valuesx.real, mode_valuesx.imag
+                )
 
                 mode_amp_int_funx = interp1d(wfx.time_axis, mode_ampx)
                 mode_amp_resamx = mode_amp_int_funx(new_time_axis)
 
                 mode_phase_int_funx = interp1d(wfx.time_axis, mode_phasex)
                 mode_phase_resamx = mode_phase_int_funx(new_time_axis)
 
@@ -292,35 +330,54 @@
                 )
 
                 # mean_phase_shift = np.mean(
                 #   mode_phase_resamx - mode_phase_resam0
                 # )
 
                 # message(mean_phase_shift)
-                delta_mode_ampx = (mode_amp_resamx - mode_amp_resam0) / mode_amp_resam0
-                delta_mode_phasex = (mode_phase_resamx - mode_phase_resam0 - mean_phase_shift) / mode_phase_resam0
+                delta_mode_ampx = (
+                    mode_amp_resamx - mode_amp_resam0
+                ) / mode_amp_resam0
+                delta_mode_phasex = (
+                    mode_phase_resamx - mode_phase_resam0 - mean_phase_shift
+                ) / mode_phase_resam0
 
-                rms_amp_diff = np.sqrt(np.sum(delta_mode_ampx**2) / (len(delta_mode_ampx)))
-                rms_phase_diff = np.sqrt(np.sum(delta_mode_phasex**2) / (len(delta_mode_phasex)))
+                rms_amp_diff = np.sqrt(
+                    np.sum(delta_mode_ampx**2) / (len(delta_mode_ampx))
+                )
+                rms_phase_diff = np.sqrt(
+                    np.sum(delta_mode_phasex**2) / (len(delta_mode_phasex))
+                )
                 max_phase_diff = np.amax(np.absolute(delta_mode_phasex))
                 max_phase_diff_loc = np.argmax(np.absolute(delta_mode_phasex))
                 max_phase_diff_time = new_time_axis[max_phase_diff_loc]
                 cumulative_diff.update(
-                    {f"l{ell}m{emm}": [rms_amp_diff, rms_phase_diff, [max_phase_diff, max_phase_diff_time]]}
+                    {
+                        f"l{ell}m{emm}": [
+                            rms_amp_diff,
+                            rms_phase_diff,
+                            [max_phase_diff, max_phase_diff_time],
+                        ]
+                    }
                 )
                 max_mode_value = np.amax(mode_values)
 
             ax1.scatter(
                 new_time_axis[:],
                 abs(delta_mode_ampx[:]),
                 label=rf"{label} $\ell${ell}$m${emm}",
                 s=1,
                 alpha=0.2 * abs(emm) % 1,
             )
-            ax2.scatter(new_time_axis[:], abs(delta_mode_phasex[:]), label=rf"{label} $\ell${ell}$m${emm}", s=1)
+            ax2.scatter(
+                new_time_axis[:],
+                abs(delta_mode_phasex[:]),
+                label=rf"{label} $\ell${ell}$m${emm}",
+                s=1,
+            )
 
     ax1.grid(which="both")
     ax2.grid(which="both")
     ax1.legend()
     ax2.legend()
     plt.tight_layout()
     ax1.set_xlabel(xlabel)
```

### Comparing `waveformtools-2023.6.5/waveformtools/diagnostics.py` & `waveformtools-2023.7.14/waveformtools/diagnostics.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import numpy as np
 
 
 class method_info:
     """The methods for integration ,differential to be passed on
     for operations."""
 
-    def __init__(self, int_method="MP", diff_method="SH", ell_max=8, degree=8, reg=True):
+    def __init__(
+        self, int_method="MP", diff_method="SH", ell_max=8, degree=8, reg=True
+    ):
         self.int_method = int_method
         self.diff_method = diff_method
         self.ell_max = ell_max
         self.reg = reg
         self.degree = degree
```

### Comparing `waveformtools-2023.6.5/waveformtools/differentiate.py` & `waveformtools-2023.7.14/waveformtools/differentiate.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,19 @@
             x_uniform = np.linspace(x_data[0], x_data[-1], 2 * len(x_data))
             y_uniform = interp1d(x_data, y_data, kind="cubic")(x_uniform)
 
         delta_x = np.diff(x_uniform)[0]
 
         if method == "FS":
             dydx_new, _, x_new, _ = Fourier_differential(
-                delta_x=delta_x, udata_x=y_uniform, order=1, zero_mode=0, taper=False
+                delta_x=delta_x,
+                udata_x=y_uniform,
+                order=1,
+                zero_mode=0,
+                taper=False,
             )
 
         elif method == "FD":
             if degree == 1:
                 dydx_new = differentiate(y_uniform, delta_x)
             elif degree == 2:
                 dydx_new = differentiate2(y_uniform, delta_x)
@@ -169,15 +173,18 @@
     # 	cheb_coeffs, result = chebfit(x_data, y_data, deg=deg_index, full=True)
     # 	res = result[0][0]
     # if res%2==0:
     # 	L2errs.append(res)
     # print(x_data, y_data)
     cheb_coeffs, result = chebfit(x_data, y_data, deg=degree, full=True)
 
-    message("Result", result, result[0], message_verbosity=1)
+    message(
+        "\n CS derivative Result\n", result, result[0], message_verbosity=4
+    )
+
     res = result[0][0]
 
     # L2errs = [(a + b)  for a, b in zip(L2errs[::2], L2errs[1::2])]
 
     # best_deg = 2*np.argmin(L2errs)+2
     # if best_deg<degree:
     # plt.plot(L2errs)
@@ -192,16 +199,20 @@
         if res <= 1e-1 and res >= 1e-3:
             message(f"Residue warning {res}")
         elif res > 1e-1:
             import traceback
 
             traceback.print_stack()
             y_fit_data = chebval(x_data, cheb_coeffs)
-            plt.scatter(x_data, y_data, label="Input", s=3, c="magenta", marker="o")
-            plt.scatter(x_data, y_fit_data, label="fit", s=3, c="blue", marker="X")
+            plt.scatter(
+                x_data, y_data, label="Input", s=3, c="magenta", marker="o"
+            )
+            plt.scatter(
+                x_data, y_fit_data, label="fit", s=3, c="blue", marker="X"
+            )
             plt.grid()
             plt.legend()
             plt.show()
 
             message(f"Residue warning {res}: Bad fit!")
 
     # compute the derivative
@@ -214,15 +225,23 @@
 
 
 ########################################################
 # Fourier differentiation
 ########################################################
 
 
-def Fourier_differential(delta_x, udata_x=None, utilde_conven=None, omega0=np.inf, order=1, zero_mode=0, taper=True):
+def Fourier_differential(
+    delta_x,
+    udata_x=None,
+    utilde_conven=None,
+    omega0=np.inf,
+    order=1,
+    zero_mode=0,
+    taper=True,
+):
     """Fixed frequency differentiation, the inverse of the
     Fixed frequency integration as presented in Reisswig et al.
     This function takes in a function and returns its nth order
     derivative differential taken in the frequency domain.
 
 
     Parameters
@@ -779,15 +798,17 @@
     # der_data = np.append(der_data, [der4], axis=aax)
     der_data[4] = der4
     for index in range(order, len(data) - order):
         # For the interior points.
         data_subarray = data[index - order : index + order + 1]
         # der_data = np.append(der_data, [np.tensordot(coeffs, data_subarray, axes=((0), (0)))
         # / (divide * delta_t)], axis=aax)
-        der_data[index] = np.tensordot(coeffs, data_subarray, axes=((0), (0))) / (divide * delta_t)
+        der_data[index] = np.tensordot(
+            coeffs, data_subarray, axes=((0), (0))
+        ) / (divide * delta_t)
 
     # der_data = np.append(der_data, [derNm5], axis=aax)
     der_data[-5] = derNm5
     # der_data = np.append(der_data, [derNm4], axis=aax)
     der_data[-4] = derNm4
     # der_data = np.append(der_data, [derNm3], axis=aax)
     der_data[-3] = derNm3
@@ -913,15 +934,17 @@
     for index in range(order, len(data) - order):
         # For the interior points.
         data_subarray = data[index - order : index + order + 1]
         # der_data = np.append(der_data, [np.tensordot(coeffs, data_subarray, axes=((0), (0)))
         # / (divide * delta_t)], axis=aax)
         # der_data[index] = np.tensordot(coeffs, data_subarray, axes=((0), (0))) / (divide * delta_t)
         for inner_index, val in enumerate(coeffs):
-            der_data[index] += val * data_subarray[inner_index] / (divide * delta_t)
+            der_data[index] += (
+                val * data_subarray[inner_index] / (divide * delta_t)
+            )
 
     # der_data = np.append(der_data, [derNm5], axis=aax)
     # der_data[-5] = derNm5
     # der_data = np.append(der_data, [derNm4], axis=aax)
     # der_data[-4] = derNm4
     # der_data = np.append(der_data, [derNm3], axis=aax)
     # der_data[-3] = derNm3
@@ -957,17 +980,25 @@
                                 The waveform differentiated in time.
 
     """
 
     # Get the amplitude and phase of the complex 1d waveform.
     from waveformtools.waveformtools import xtract_camp_phase
 
-    waveform_amp, waveform_phase = xtract_camp_phase(waveform.real, waveform.imag)
+    waveform_amp, waveform_phase = xtract_camp_phase(
+        waveform.real, waveform.imag
+    )
 
     # Differentiate the waveform.
 
-    Amplitude_dot = derivative(time_axis, waveform_amp, method=method, degree=degree)
-    Phase_dot = derivative(time_axis, waveform_phase, method=method, degree=degree)
-
-    differentiated_waveform = (Amplitude_dot + waveform_amp * 1j * Phase_dot) * np.exp(1j * waveform_phase)
+    Amplitude_dot = derivative(
+        time_axis, waveform_amp, method=method, degree=degree
+    )
+    Phase_dot = derivative(
+        time_axis, waveform_phase, method=method, degree=degree
+    )
+
+    differentiated_waveform = (
+        Amplitude_dot + waveform_amp * 1j * Phase_dot
+    ) * np.exp(1j * waveform_phase)
 
     return differentiated_waveform
```

### Comparing `waveformtools-2023.6.5/waveformtools/extrapolate.py` & `waveformtools-2023.7.14/waveformtools/extrapolate.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,26 +48,38 @@
 
     References
     ----------
 
     Nakano et al., (2015),	Phys. Rev. D 91, 104022, in-text below Eq.[30].
     """
 
-    areal_radius = coord_radius * (1 + (mass + spin) / (2 * coord_radius)) * (1 + (mass - spin) / (2 * coord_radius))
+    areal_radius = (
+        coord_radius
+        * (1 + (mass + spin) / (2 * coord_radius))
+        * (1 + (mass - spin) / (2 * coord_radius))
+    )
 
     return areal_radius
 
 
 ############################################################################
 # Perturbative extraction
 ############################################################################
 
 
 def waveextract_to_inf_perturbative_twop5_order(
-    rPsi4_rlm, delta_t, areal_radius=500, mass=1, spin=0, ell=2, emm=2, degree=24, method="CS"
+    rPsi4_rlm,
+    delta_t,
+    areal_radius=500,
+    mass=1,
+    spin=0,
+    ell=2,
+    emm=2,
+    degree=24,
+    method="CS",
 ):
     """Extract a numerical waveform to null infinity using perturbative techniques. This is :
             * accurate to second order in :math:`1/r`.
             * accurate to first order in Kerr mass and spin.
             * corrects for spheroidal harmonics
 
 
@@ -114,44 +126,63 @@
     # Timeaxis
 
     timeaxis = np.arange(0, len(rPsi4_rlm) * delta_t, delta_t)
     # Assigning the terms. Each set of subterms in a pair of paranthesis is a term.
     term_1_prefac = 1 - 2 * mass / areal_radius
     subterm_1_1 = rPsi4_rlm
     subterm_1_2_prefac = (ell - 1) * (ell + 2) / (2 * areal_radius)
-    subterm_1_2, _ = fixed_frequency_integrator(rPsi4_rlm, delta_t, omega0=0.015)  # Integral_rPsi4_rlm
-    subterm_1_3_prefac = (ell - 1) * (ell + 2) * (ell**2 + ell - 4) / (8 * areal_radius**2)
-    subterm_1_3, _ = fixed_frequency_integrator(rPsi4_rlm, delta_t, order=2, omega0=0.015)  # Double_integral_rPsi4_rlm
-
-    term_1 = term_1_prefac * (subterm_1_1 + subterm_1_2_prefac * subterm_1_2 + subterm_1_3_prefac * subterm_1_3)
+    subterm_1_2, _ = fixed_frequency_integrator(
+        rPsi4_rlm, delta_t, omega0=0.015
+    )  # Integral_rPsi4_rlm
+    subterm_1_3_prefac = (
+        (ell - 1) * (ell + 2) * (ell**2 + ell - 4) / (8 * areal_radius**2)
+    )
+    subterm_1_3, _ = fixed_frequency_integrator(
+        rPsi4_rlm, delta_t, order=2, omega0=0.015
+    )  # Double_integral_rPsi4_rlm
+
+    term_1 = term_1_prefac * (
+        subterm_1_1
+        + subterm_1_2_prefac * subterm_1_2
+        + subterm_1_3_prefac * subterm_1_3
+    )
 
     term_2_prefac = (2 * 1j * spin / (ell + 1) ** 2) * np.sqrt(
-        (ell + 3) * (ell - 1) * (ell + emm + 1) * (ell - emm + 1) / ((2 * ell + 1) * (2 * ell + 3))
+        (ell + 3)
+        * (ell - 1)
+        * (ell + emm + 1)
+        * (ell - emm + 1)
+        / ((2 * ell + 1) * (2 * ell + 3))
     )
-    subterm_2_1 = differentiate_cwaveform(timeaxis, rPsi4_rlm, method=method, degree=degree)  # Differential of waveform
+    subterm_2_1 = differentiate_cwaveform(
+        timeaxis, rPsi4_rlm, method=method, degree=degree
+    )  # Differential of waveform
     subterm_2_2_prefac = -ell * (ell + 3) / areal_radius
     subterm_2_2 = subterm_1_1
 
     term_2 = term_2_prefac * (subterm_2_1 + subterm_2_2_prefac * subterm_2_2)
 
     term_3_prefac = (-2 * 1j * spin / ell**2) * np.sqrt(
-        ((ell + 2) * (ell - 2) * (ell + emm) * (ell - emm)) / ((2 * ell - 1) * (2 * ell + 1))
+        ((ell + 2) * (ell - 2) * (ell + emm) * (ell - emm))
+        / ((2 * ell - 1) * (2 * ell + 1))
     )
     subterm_3_1 = subterm_2_1
     subterm_3_2_prefac = -(ell - 2) * (ell + 1) / areal_radius
     subterm_3_2 = subterm_1_1
 
     term_3 = term_3_prefac * (subterm_3_1 + subterm_3_2_prefac * subterm_3_2)
 
     rPsi4_inflm = term_1 + term_2 + term_3
 
     return rPsi4_inflm
 
 
-def waveextract_to_inf_perturbative_two_order(rPsi4_rlm, delta_t, areal_radius=500, mass=1, ell=2):
+def waveextract_to_inf_perturbative_two_order(
+    rPsi4_rlm, delta_t, areal_radius=500, mass=1, ell=2
+):
     """Extract a numerical waveform to null infinity using perturbative techniques. This is :
             * accurate to second order in :math:`1/r`.
             * accurate to first order in Kerr mass and spin.
             * corrects for spheroidal harmonics
 
 
 
@@ -197,31 +228,39 @@
 
     from integrate import fixed_frequency_integrator
 
     # Assigning the terms. Each set of subterms in a pair of paranthesis is a term.
     term_1 = rPsi4_rlm
 
     term_2_prefac = -(ell - 1) * (ell + 2) / (2 * areal_radius)
-    subterm_2_1, _ = fixed_frequency_integrator(rPsi4_rlm, delta_t, omega0=0.015)  # Integral_rPsi4_rlm
+    subterm_2_1, _ = fixed_frequency_integrator(
+        rPsi4_rlm, delta_t, omega0=0.015
+    )  # Integral_rPsi4_rlm
     term_2 = term_2_prefac * subterm_2_1
 
-    term_3_prefac = (ell - 1) * (ell + 2) * (ell**2 + ell - 4) / (8 * areal_radius**2)
-    subterm_3_1, _ = fixed_frequency_integrator(rPsi4_rlm, delta_t, order=2, omega0=0.015)  # Double_Integral_rPsi4_rlm
+    term_3_prefac = (
+        (ell - 1) * (ell + 2) * (ell**2 + ell - 4) / (8 * areal_radius**2)
+    )
+    subterm_3_1, _ = fixed_frequency_integrator(
+        rPsi4_rlm, delta_t, order=2, omega0=0.015
+    )  # Double_Integral_rPsi4_rlm
     term_3 = term_3_prefac * subterm_3_1
 
     term_4_prefac = -3 * mass / (2 * areal_radius**2)
     subterm_4_1 = subterm_2_1
     term_4 = term_4_prefac * subterm_4_1
 
     rPsi4_inflm = term_1 + term_2 + term_3 + term_4
 
     return rPsi4_inflm
 
 
-def waveextract_to_inf_perturbative_one_order(u_ret, rPsi4_rlm, areal_radius=500, ell=2):
+def waveextract_to_inf_perturbative_one_order(
+    u_ret, rPsi4_rlm, areal_radius=500, ell=2
+):
     """Extract a numerical waveform to null infinity using perturbative techniques. This is :
             * accurate to second order in :math:`1/r`.
             * accurate to first order in Kerr mass and spin.
             * corrects for spheroidal harmonics
 
 
 
@@ -265,20 +304,24 @@
     # Get the amplitude and phase
     A_lm, _ = waveformtools.xtract_camp_phase(rPsi4_rlm.real, rPsi4_rlm.imag)
 
     # Get the time stepping
     delta_t = u_ret[1] - u_ret[0]
 
     # Get the waveform instantaneous frequency
-    omega_lm = waveformtools.get_waveform_angular_frequency(rPsi4_rlm, delta_t=delta_t, timeaxis=u_ret)
+    omega_lm = waveformtools.get_waveform_angular_frequency(
+        rPsi4_rlm, delta_t=delta_t, timeaxis=u_ret
+    )
 
     # Assigning the terms. Each set of subterms in a pair of paranthesis is a term.
 
     # The amplitude correction factor
-    A_lm_correction = 0.5 * np.power(((ell * (ell + 1) / (2 * omega_lm * areal_radius))), 2)
+    A_lm_correction = 0.5 * np.power(
+        ((ell * (ell + 1) / (2 * omega_lm * areal_radius))), 2
+    )
 
     # The phase correction factor.
     sin_Phase_correction = ell * (ell + 1) / (2 * omega_lm * areal_radius)
     cos_Phase_correction = np.sqrt(1 - np.power(sin_Phase_correction, 2))
     Phase_correction = cos_Phase_correction + 1j * sin_Phase_correction
 
     # The extrapolated waveform
```

### Comparing `waveformtools-2023.6.5/waveformtools/grids.py` & `waveformtools-2023.7.14/waveformtools/grids.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,286 +1,277 @@
 """ Classes to hold grid information
 
 
 Classes
 -------
-spherical_grid: grid info.
-                Stores information on the 2d grid in spherical polar coordinates.
-gl_grid : grid info
-          Stores a Gauss-Legendre type grid on a spherical surface.
+UniformGrid : grid info.
+              Stores information on the 2d grid in spherical polar coordinates.
+GLGrid : grid info
+         Stores a Gauss-Legendre type grid on a spherical surface.
 """
 
 import numpy as np
 
 # from numba import jit, njit
 
 # import numba as nb
 
 # from numba.experimental import jitclass
 
 
-class spherical_grid:
-    """A class to store the coordinate grid on a sphere.
-
-    Attributes
-    ----------
-    ntheta: int
-                            The number of angular points in the :math:`\\theta`
-                            direction, including ghost zones.
-    nphi:   int
-                    The number of angular points in the :math:`\\phi`
-                    direction, including ghost zones.
-    nghosts:    int
-                            The number of ghost zones at the end of
-                            each direction.
-    meshgrid:   tuple of 2d array
-                            The 2d array containing the meshgrid of
-                            (:math:`\\theta, \\phi`) angular points.
-    theta_1d:   1d array
-                            The 1d array of angular points
-                            along the :math:`\\theta` axis.
-    phi_1d: 1d array
-                            The 1d array of angular points
-                            along the :math:`\\phi` axis.
-    dtheta: float
-                            The angular step size in the :math:`\\theta`
-                            direction.
-    dphi:   float
-                    The angular step size inthe :math:`\\phi`
-                    direction.
-    npix_act:   int
-                            The total number of gridpoints on the sphere,
-                            excluding the ghost points.
-    meshgrid:
-                            Get the 2d angular grid.
-
-    Methods
-    -------
-    theta_1d:
-                            Get the :math:`\\theta` axis.
-    phi_1d:
-                            Get the :math:`\\phi` axis.
+class UniformGrid:
+    """A class to store the theta-phi grid info."""
 
-    """
+    def __init__(
+        self,
+        nphi=80,
+        ntheta=41,
+        nphimax=124,
+        nthetamax=66,
+        nghosts=2,
+        integration_method="MP",
+    ):
 
-    def __init__(self, nphi=80, ntheta=41, nphimax=124, nthetamax=66, nghosts=2):
         # Number of gridpoints along phi direction including ghost points.
         self.nphi = nphi
         # Number of gridpoints along theta direction including ghost points.
         self.ntheta = ntheta
         # Total length of phi array used by ETK.
         self.nphimax = nphimax
         # Total length of theta array used by ETK.
         self.nthetamax = nthetamax
         # Number of ghost points in theta/phi direction.
         self.nghosts = nghosts
+        # The default integration method
+        self._integration_method = integration_method
 
     @property
     def npix(self):
-        """Return the total number of pixels,
-        including the ghost zones present
-        at one iteration."""
+        # Return the total number of pixels, including the ghost zones present at one iteration.
         return (self.ntheta) * (self.nphi)
 
     @property
     def npix_act(self):
-        """Return the actual number of pixels,
-        excluding the ghost zones present at
-        one iteration"""
-        return (self.ntheta - 2 * self.nghosts) * (self.nphi - 2 * self.nghosts)
+        # Return the actual number of pixels, excluding the ghost zones present at one iteration.
+        return (self.ntheta - 2 * self.nghosts) * (
+            self.nphi - 2 * self.nghosts
+        )
 
     @property
     def npix_max(self):
-        """Return the (max) total number of pixels,
-        including the ghost and buffer zones at
-        one iteration."""
+        # Return the (max) total number of pixels, including the ghost and buffer zones at one iteration.
         return (self.nthetamax) * (self.nphimax)
 
     @property
     def ntheta_act(self):
         """Return the actual number of valid pixels,
-        excluding the ghost and buffer zones, along
-        the theta axis at one iteration."""
-
+        excluding the ghost and buffer zones, along the
+        theta axis at one iteration."""
         return self.ntheta - 2 * self.nghosts
 
     @property
     def nphi_act(self):
         """Return the actual number of valid pixels,
-        excluding the ghost and buffer zones, along
-        the phi axis at one iteration."""
+        excluding the ghost and buffer zones,
+        along the phi axis at one iteration."""
         return self.nphi - 2 * self.nghosts
 
     @property
     def dtheta(self):
-        """Return the coodinate spacing :math:`d\\theta.`"""
+        # Return the coodinate spacing d\theta
         return np.pi / (self.ntheta - 2 * self.nghosts)
 
     @property
     def dphi(self):
-        """Return the coordinate spacing :math:`d\\phi`."""
+        # Return the coordinate spacing d\phi
         return 2 * np.pi / (self.nphi - 2 * self.nghosts)
 
     @property
     def nbuffer(self):
-        """Return the number of buffer zones (excluding ghosts)"""
+        # Return the coordinate spacing d\phi
         return self.nthetamax - self.ntheta
 
+    @property
+    def shape(self):
+        """Return the shape of the grif"""
+        return (self.ntheta_act, self.nphi_act)
+
+    @property
     def theta_1d(self, theta_index=None):
-        """Returns the coordinate value theta given
-        the coordinate index. The coordinate index
-        ranges from (0, ntheta). The actual indices
-        without the ghost and extra zones
+        """Returns the coordinate value theta 
+        given the coordinate index. The coordinate 
+        index ranges from (0, ntheta). The actual 
+        indices without the ghost and extra zones 
         is (nghosts, ntheta-nghosts).
 
         Parameters
         -----------
-
-        theta_index:    int/ 1d array
-                                        The theta coordinate index or axis.
+        theta_index : int/ 1d array
+                      The theta coordinate index or axis.
 
         Returns
         -------
-
-        theta_1d:   float
-                                The coordinate(s) :math:`\\theta` on the sphere.
-
+        theta_1d : float
+                   The coordinate(s) :math:`\\theta` on the sphere.
         """
 
         if not theta_index:
             theta_index = np.arange(self.nghosts, self.ntheta - self.nghosts)
 
-        return (theta_index - self.nghosts + 0.5) * np.pi / (self.ntheta - 2 * self.nghosts)
+        return (
+            (theta_index - self.nghosts + 0.5)
+            * np.pi
+            / (self.ntheta - 2 * self.nghosts)
+        )
 
+    @property
     def phi_1d(self, phi_index=None):
-        """Returns the coordinate value theta
-        given the coordinate index. The coordinate
-        index lies in (0, nphi). The actual indices
-        without the ghost and extra zones
-        is (nghosts, nphi-nghosts).
+        """Returns the coordinate value theta given 
+        the coordinate index. The coordinate index lies 
+        in (0, nphi). The actual indices without 
+        the ghost and extra zones is (nghosts, nphi-nghosts).
 
         Parameters
         -----------
-
-        phi_1d: int / 1d array
-                                The phi coordinate index or axis.
+        phi_1d : int / 1d array
+                 The phi coordinate index or axis.
 
         Returns
         -------
-
-        phi_1d: float or 1d array
-                                The coordinate(s) :math:`\\phi` on the sphere.
+        phi_1d : float or 1d array
+                 The coordinate(s) :math:`\\phi` on the sphere.
 
         """
 
         if not phi_index:
             phi_index = np.arange(self.nghosts, self.nphi - self.nghosts)
 
-        return (phi_index - self.nghosts) * 2 * np.pi / (self.nphi - 2 * self.nghosts)
+        return (
+            (phi_index - self.nghosts)
+            * 2
+            * np.pi
+            / (self.nphi - 2 * self.nghosts)
+        )
 
     @property
     def meshgrid(self):
         """The (:math:`\\theta, \\phi)`: coordinate meshes.
-                Excludes the ghost zones.
-
+        Excludes the ghost zones.
 
         Returns
         -------
-
-        theta:  2d array
-                        The :math:`\\theta` coordinate matrix for vectorization.
-
-        phi:    2d array
-                        The :math:`\\phi` coordinate matrix for vectorization.
-
+        theta :	2d array
+                The :math:`\\theta` coordinate matrix 
+                for vectorization.
+
+        phi : 2d array
+              The :math:`\\phi` coordinate matrix 
+              for vectorization.
         """
 
-        theta, phi = np.meshgrid(self.theta_1d(), self.phi_1d())
+        theta, phi = np.meshgrid(self.theta_1d, self.phi_1d)
 
         # theta = np.zeros((self.ntheta_act, self.nphi_act))
-        # phi   = np.zeros((self.ntheta_act, self.nphi_act))
+        # phi	= np.zeros((self.ntheta_act, self.nphi_act))
 
         # for theta_index, theta_val in enumerate(self.theta_1d()):
-        #   for phi_index, phi_val in enumerate(self.phi_1d()):
-        #       theta[theta_index, phi_index] = theta_val
-        #       phi[theta_index, phi_index] = phi_val
+        # 	for phi_index, phi_val in enumerate(self.phi_1d()):
+        # 		theta[theta_index, phi_index] = theta_val
+        # 		phi[theta_index, phi_index] = phi_val
 
         return np.transpose(theta), np.transpose(phi)
 
+    @property
+    def integration_method(self):
+        """The default integration method"""
+        return self._integration_method
+
 
-class gl_grid:
+class GLGrid:
     """A class to store the coordinate grid on a sphere.
 
     Attributes
     ----------
-    ntheta: int
-                The number of angular points in the :math:`\\theta`
-                direction, including ghost zones.
-    nphi:   int
-            The number of angular points in the :math:`\\phi`
-            direction, including ghost zones.
-    nghosts:    int
-                The number of ghost zones at the end of
-                each direction.
-    meshgrid:   tuple of 2d array
-                The 2d array containing the meshgrid of
-                (:math:`\\theta, \\phi`) angular points.
-    theta_1d:   1d array
-                The 1d array of angular points
-                along the :math:`\\theta` axis.
-    phi_1d: 1d array
-                The 1d array of angular points
-                along the :math:`\\phi` axis.
-    dtheta: float
-                The angular step size in the :math:`\\theta`
-                direction.
-    dphi:   float
-            The angular step size inthe :math:`\\phi`
-            direction.
-    npix_act:   int
-                The total number of gridpoints on the sphere,
-                excluding the ghost points.
-    meshgrid:
-                Get the 2d angular grid.
+    ntheta : int
+             The number of angular points in the :math:`\\theta`
+             direction, including ghost zones.
+    nphi : int
+           The number of angular points in the :math:`\\phi`
+           direction, including ghost zones.
+    nghosts : int
+              The number of ghost zones at the end of
+              each direction.
+    meshgrid : tuple of 2d array
+               The 2d array containing the meshgrid of
+               (:math:`\\theta, \\phi`) angular points.
+    theta_1d : 1d array
+               The 1d array of angular points
+               along the :math:`\\theta` axis.
+    phi_1d : 1d array
+             The 1d array of angular points
+             along the :math:`\\phi` axis.
+    dtheta : float
+             The angular step size in the :math:`\\theta`
+             direction.
+    dphi : float
+           The angular step size inthe :math:`\\phi`
+           direction.
+    npix_act : int
+               The total number of gridpoints on the sphere,
+               excluding the ghost points.
+    meshgrid : tuple of 2darray
+               Get the 2d angular grid.
 
     Methods
     -------
-    theta_1d:
-                Get the :math:`\\theta` axis.
-    phi_1d:
-                Get the :math:`\\phi` axis.
+    theta_1d :
+        Get the :math:`\\theta` axis.
+    phi_1d :
+        Get the :math:`\\phi` axis.
 
     Notes
     -----
-
-    The total number of points on the sphere is assumed to be :math:`(L+1)^2`
+    The total number of points on the sphere
+    is assumed to be :math:`2 (L+1)^2`
 
     :math:`N_\theta = L+1`
 
     :math:`N_\phi = 2(L+1)`
 
     This integrates out spherical harmonics of degree L exactly,
     given a regular function on the sphere.
     """
 
-    def __init__(self, nphi=None, ntheta=None, L=47, nghosts=2):
+    def __init__(
+        self,
+        nphi=None,
+        ntheta=None,
+        nphi_act=None,
+        ntheta_act=None,
+        L=47,
+        nghosts=2,
+        integration_method="GL"):
+
         # Number of gridpoints along phi direction including ghost points.
         self._nphi = nphi
         # Number of gridpoints along theta direction including ghost points.
         self._ntheta = ntheta
+        self._nphi_act = nphi_act
+        self._ntheta_act = ntheta_act
         # Total length of phi array used by ETK.
-        # self._nphimax   = nphimax
+        # self._nphimax		= nphimax
         # Total length of theta array used by ETK.
-        # self._nthetamax = nthetamax
+        # self._nthetamax	= nthetamax
         # Number of ghost points in theta/phi direction.
         self._nghosts = nghosts
         self._L = L
         self._theta_1d = None
         self._phi_1d = None
         self._meshgrid = None
+        self._integration_method = integration_method
 
         if self._ntheta is None:
             if self._L is None:
                 raise ValueError("Please specify L or angular points!")
 
             else:
                 self._ntheta_act = L + 1
@@ -289,20 +280,23 @@
                 self._ntheta = self._ntheta_act + 2 * self._nghosts
                 self._nphi = self._nphi_act + 2 * self._nghosts
 
         elif self._L is None:
             if self.nthetha is None:
                 raise ValueError("Please specify L or angular points!")
             else:
-                self.L = self.ntheta - 1
-                assert nphi % 2 == 0
+                self.L = self.ntheta_act - 1
+                # assert(nphi%2==0)
+                self.nphi_act = 2 * self.L + 1
 
         from scipy.special import roots_legendre
 
-        cpoints, self._weights, self._sum_of_weights = roots_legendre(L + 1, mu=True)
+        cpoints, self._weights, self._sum_of_weights = roots_legendre(
+            L + 1, mu=True
+        )
 
         # xpoints = (np.pi-np.arccos(cpoints))
         xpoints = np.arccos(cpoints[::-1])
         self._theta_1d = xpoints
 
         dphi = 2 * np.pi / self._nphi_act
 
@@ -316,150 +310,156 @@
         dtheta_axis = np.append(dtheta_axis, np.pi - self._theta_1d[-1])
         dtheta_axis = np.insert(dtheta_axis, 0, self._theta_1d[0])
 
         self._dtheta_1d = dtheta_axis
 
         self._dphi = dphi  # self._phi_1d[1]
 
-    @property
     def nphi(self):
-        """Return the (max) total number of pixels,
-        including the ghost and buffer zones at
-        one iteration."""
-        return self._nphi
+        """Return the total number of gridpoints
+        along the phi direction, including
+        the ghost zones at one iteration."""
+        if not self._nphi:
+            return self._nphi_act + self.nghosts
+        else:
+            return self._nphi
 
-    @property
     def ntheta(self):
-        """Return the actual number of valid pixels,
-        excluding the ghost and buffer zones, along
-        the theta axis at one iteration."""
-        return self._ntheta
+        """Return the total number gridpoints
+        along the theta direction, including
+        the ghost zones at one iteration."""
+        if not self._ntheta:
+            return self._ntheta_act + self.nghosts
+        else:
+            return self._ntheta
 
     @property
     def nghosts(self):
-        """Return the number of ghost zones at each end in each direction"""
+        """Return the number of ghost zones
+        at each end in each direction"""
         return self._nghosts
 
     @property
     def ntheta_act(self):
-        """Return the actual number of valid pixels,
-        excluding the ghost and buffer zones, along
-        the phi axis at one iteration."""
-        return self.ntheta - 2 * self.nghosts
+        """Return the actual number of physical data points
+        along the theta direction excluding the ghost and
+        buffer zones at one iteration."""
+        if not self._ntheta_act:
+            return self.ntheta - 2 * self.nghosts
+        else:
+            return self._ntheta_act
 
     @property
     def nphi_act(self):
-        """Return the actual number of valid pixels,
-        excluding the ghost and buffer zones, along
-        the phi axis at one iteration."""
-        return self.nphi - 2 * self.nghosts
+        """Return the actual number of physical data points
+        along the phi direction excluding the ghost and
+        buffer zones at one iteration."""
+
+        if not self._ntheta_act:
+            return self.nphi - 2 * self.nghosts
+        else:
+            return self._nphi_act
 
     @property
     def npix_act(self):
         """Return the actual number of pixels,
-        excluding the ghost zones present at
-        one iteration"""
+        excluding the ghost zones present
+        at one iteration"""
         return (self.ntheta_act) * (self.nphi_act)
 
     @property
     def dtheta_1d(self):
-        """Return the non-uniform angular stepping
-        in :math:`\theta` direction"""
+        """Return the non-uniform angular stepping in 
+        :math:`\theta` direction"""
         return self._dtheta_1d
 
     @property
     def dphi(self):
-        """Return the uniform angular stepping
-        in :math:`\phi` direction"""
+        """Return the uniform angular stepping in :math:`\phi` direction"""
         return self._dphi
 
     @property
     def L(self):
-        """Return the maximum mode number
-        that this grid can integrate out."""
-
+        """Return the total number of pixels, including 
+        the ghost zones present at one iteration."""
         return self._L
 
     @property
     def npix(self):
-        """Return the total number of pixels,
-        including the ghost zones present at
-        one iteration."""
+        """Return the total number of pixels, including 
+        the ghost zones present at one iteration."""
         return (self.ntheta) * (self.nphi)
 
     @property
     def weights(self):
-        """Return the integration weights along theta."""
+        """Return the integration weights along theta"""
         return self._weights
 
     @property
     def weights_grid(self):
         """Return the integration weights on the coordinate mesh grid"""
         return np.outer(self.weights, np.ones(self.nphi_act))
 
     @property
     def shape(self):
-        """Return the shape of the grid."""
+        """Return the shape of the grif"""
         return self.weights_grid.shape
 
     @property
     def theta_1d(self):
-        """Returns the coordinate values theta given the coordinate index.
-        The coordinate index ranges from (0, ntheta). The actual indices
+        """Returns the coordinate value theta given the coordinate index. 
+        The coordinate index ranges from (0, ntheta). The actual indices 
         without the ghost and extra zones is (nghosts, ntheta-nghosts).
 
         Parameters
         -----------
-
-        theta_index:    int/ 1d array
-                        The theta coordinate index or axis.
+        theta_index : int/ 1d array
+                      The theta coordinate index or axis.
 
         Returns
         -------
-
-        theta_1d:   float
-                    The coordinate(s) :math:`\\theta` on the sphere.
-
+        theta_1d : float
+                   The coordinate(s) :math:`\\theta` on the sphere.
         """
 
         return self._theta_1d
 
     @property
     def phi_1d(self):
-        """Returns the coordinate values phi given the coordinate index.
-        The coordinate index lies in (0, nphi). The actual indices without
+        """Returns the coordinate value theta given the coordinate index. 
+        The coordinate index lies in (0, nphi). The actual indices without 
         the ghost and extra zones is (nghosts, nphi-nghosts).
 
         Parameters
         -----------
-
-        phi_1d: int / 1d array
-                    The phi coordinate index or axis.
+        phi_1d : int / 1d array
+                 The phi coordinate index or axis.
 
         Returns
         -------
-
-        phi_1d: float or 1d array
-                    The coordinate(s) :math:`\\phi` on the sphere.
-
+        phi_1d : float or 1d array
+                 The coordinate(s) :math:`\\phi` on the sphere.
         """
 
         return self._phi_1d
 
     @property
     def meshgrid(self):
         """The (:math:`\\theta, \\phi)`: coordinate meshes.
-            Excludes the ghost zones.
+        Excludes the ghost zones.
 
 
         Returns
         -------
-
-        theta:  2d array
+        theta :	2d array
                 The :math:`\\theta` coordinate matrix for vectorization.
 
-        phi:    2d array
-                The :math:`\\phi` coordinate matrix for vectorization.
-
+        phi : 2d array
+              The :math:`\\phi` coordinate matrix for vectorization.
         """
 
         return self._meshgrid
+
+    @property
+    def integration_method(self):
+        """The default integration method"""
+        return self._integration_method
```

### Comparing `waveformtools-2023.6.5/waveformtools/integrate.py` & `waveformtools-2023.7.14/waveformtools/integrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 from waveformtools.waveformtools import message
 
 ##################################################
 # Fixed frequency integration
 ##################################################
 
 
-def fixed_frequency_integrator(udata_time, delta_t, utilde_conven=None, omega0=0, order=1, zero_mode=0):
+def fixed_frequency_integrator(
+    udata_time, delta_t, utilde_conven=None, omega0=0, order=1, zero_mode=0
+):
     """Fixed frequency integrator as presented in Reisswig et. al.
 
 
     Parameters
     ----------
     udata_time:	1d array
                             The input data in time.
@@ -296,31 +298,46 @@
     assert NTheta % 2 == 0
     assert NPhi % 2 == 0
 
     Px = int(NTheta / 2)
     Py = int(NPhi / 2)
 
     # Around corners
-    integrand_sum += func[0, 0] + func[NTheta - 1, 0] + func[0, NPhi - 1] + func[NTheta - 1, NPhi - 1]
+    integrand_sum += (
+        func[0, 0]
+        + func[NTheta - 1, 0]
+        + func[0, NPhi - 1]
+        + func[NTheta - 1, NPhi - 1]
+    )
 
     # Arount edges
     for index_phi in range(1, Py):
-        integrand_sum += 4 * func[0, 2 * index_phi - 1] + 4 * func[NTheta - 1, 2 * index_phi - 1]
+        integrand_sum += (
+            4 * func[0, 2 * index_phi - 1]
+            + 4 * func[NTheta - 1, 2 * index_phi - 1]
+        )
 
     # for (iy = 1; iy <= py-1; iy++)
     for index_phi in range(1, Py - 1):
-        integrand_sum += 2 * func[0, 2 * index_phi] + 2 * func[NTheta - 1, 2 * index_phi]
+        integrand_sum += (
+            2 * func[0, 2 * index_phi] + 2 * func[NTheta - 1, 2 * index_phi]
+        )
 
     # for (ix = 1; ix <= px; ix++)
     for index_theta in range(1, Px):
-        integrand_sum += 4 * func[2 * index_theta - 1, 0] + 4 * func[2 * index_theta - 1, NPhi - 1]
+        integrand_sum += (
+            4 * func[2 * index_theta - 1, 0]
+            + 4 * func[2 * index_theta - 1, NPhi - 1]
+        )
 
     # for (ix = 1; ix <= px-1; ix++)
     for index_theta in range(1, Px - 1):
-        integrand_sum += 2 * func[2 * index_theta, 0] + 2 * func[2 * index_theta, NPhi - 1]
+        integrand_sum += (
+            2 * func[2 * index_theta, 0] + 2 * func[2 * index_theta, NPhi - 1]
+        )
 
     # In the Interiors
     # for (iy = 1; iy <= py; iy++)
     for index_phi in range(1, Py):
         # for (ix = 1; ix <= px; ix++)
         for index_theta in range(1, Px):
             integrand_sum += 16 * func[2 * index_theta - 1, 2 * index_phi - 1]
```

### Comparing `waveformtools-2023.6.5/waveformtools/legacy.py` & `waveformtools-2023.7.14/waveformtools/legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,30 +85,36 @@
     # Iterate over (signal,template) pairs in waveforms
     for waveformdat in waveforms:
         # Carryout the match
         if not delt:
             try:
                 delt = waveformdat[0].delta_t
             except BaseException:
-                message("Waveform is not a pycbc TimeSeries. Please provide the gridspacing delt")
+                message(
+                    "Waveform is not a pycbc TimeSeries. Please provide the gridspacing delt"
+                )
                 sys.exit(0)
         # Match procedure
 
         # signaldat = lengtheq(waveformdat[0], waveformdat[1], delt)
 
         # waveform1 = signaldat[0]
         # waveform2 = signaldat[1]
-        waveform1, waveform2, _ = lengtheq(waveformdat[0], waveformdat[1], delt, is_ts=True)
+        waveform1, waveform2, _ = lengtheq(
+            waveformdat[0], waveformdat[1], delt, is_ts=True
+        )
 
         # alignedwvs = pycbc.waveform.utils.coalign_waveforms(signaldat,hpa)
         # Compute the match to calculate match and shift.
         # Note: The match function from pycbc returns the match of the
         # normalized templates
 
-        (match_score, shift) = pycbc.filter.matchedfilter.match(waveform1, waveform2)
+        (match_score, shift) = pycbc.filter.matchedfilter.match(
+            waveform1, waveform2
+        )
 
         message("Priliminary match", match_score, shift)
         # Shift the matched data against the template using the shift obtained
         # above
         waveform1 = roll(np.array(waveform1), int(shift))
         # waveform1 = shiftmatched(np.array(waveform1), int(shift), delt)
         # Compute the start and end of the non-zero signal
@@ -121,22 +127,26 @@
             message("Absolute startend not found. Fixing approximate startend")
         # Match procedure
 
         # signaldat = lengtheq(waveformdat[0], waveformdat[1], delt)
 
         # waveform1 = signaldat[0]
         # waveform2 = signaldat[1]
-        waveform1, waveform2, _ = lengtheq(waveformdat[0], waveformdat[1], delt, is_ts=True)
+        waveform1, waveform2, _ = lengtheq(
+            waveformdat[0], waveformdat[1], delt, is_ts=True
+        )
 
         # alignedwvs = pycbc.waveform.utils.coalign_waveforms(signaldat,hpa)
         # Compute the match to calculate match and shift.
         # Note: The match function from pycbc returns the match of the
         # normalized templates
 
-        (match_score, shift) = pycbc.filter.matchedfilter.match(waveform1, waveform2)
+        (match_score, shift) = pycbc.filter.matchedfilter.match(
+            waveform1, waveform2
+        )
 
         message("Priliminary match", match_score, shift)
         # Shift the matched data against the template using the shift obtained
         # above
         waveform1 = roll(np.array(waveform1), int(shift))
         # waveform1 = shiftmatched(np.array(waveform1), int(shift), delt)
         # Compute the start and end of the non-zero signal
@@ -146,42 +156,62 @@
         try:
             starti, endi = startend(waveform1)
         except BaseException:
             message("Absolute startend not found. Fixing approximate startend")
             starti, endi = apxstartend(waveform1)
             message("starti, endi")
 
-        message("The approximate start and end indices are", starti, endi, "length", endi - starti)
+        message(
+            "The approximate start and end indices are",
+            starti,
+            endi,
+            "length",
+            endi - starti,
+        )
         # Convert the non-zero portion of the signal and template to
         # time-series
         message("Converting shifted vectors to time series")
         signal = pycbc.types.timeseries.TimeSeries(
-            np.array(waveform1)[starti:endi] / np.linalg.norm(np.array(waveform1)[starti:endi]), delt
+            np.array(waveform1)[starti:endi]
+            / np.linalg.norm(np.array(waveform1)[starti:endi]),
+            delt,
         )
         template = pycbc.types.timeseries.TimeSeries(
-            np.array(waveform2)[starti:endi] / np.linalg.norm(np.array(waveform2)[starti:endi]), delt
+            np.array(waveform2)[starti:endi]
+            / np.linalg.norm(np.array(waveform2)[starti:endi]),
+            delt,
         )
         # Sanity check: The template and the signal must be of the same length
         # at this point in execution
         if len(signal) != len(template):
             message("Error\n")
-            message("Length of data, template after truncation are %d,%d" % (len(signal), len(template)))
+            message(
+                "Length of data, template after truncation are %d,%d"
+                % (len(signal), len(template))
+            )
             sys.exit(0)
         # Compute the match, shift again on the truncated data
         # message("length of data %d, aligned data %d, template %d",
         # (len(signaldat),len(alignedwvs[0]),len(alignedwvs[1])))
 
         try:
-            (match_score, shift) = pycbc.filter.matchedfilter.match(signal, template)
+            (match_score, shift) = pycbc.filter.matchedfilter.match(
+                signal, template
+            )
         except BaseException:
             message("Final match couldn't be found!")
             match_score = None
             shift = None
 
-        match = {"Match score": match_score, "Shift": shift, "Start index": starti, "End index": endi}
+        match = {
+            "Match score": match_score,
+            "Shift": shift,
+            "Start index": starti,
+            "End index": endi,
+        }
     return match
 
 
 def iscontinuous_old(timeaxis, delta_t=0):
     """Check if the data has discontinuities. This checks for repetitive time rows and jumps.
 
     Notes
@@ -241,15 +271,17 @@
             # Repetitive rows
             if timestamp < timeaxis[0] + epoch_index * delta_t:
                 discontinuity_type = 1
             # Missing rows
             elif epoch > timeaxis[0] + epoch_index + delta_t:
                 discontinuity_type = 2
             # Append [index location,correct timestamp
-            discontinuity_details.append([epoch_index, timeaxis[epoch_index], discontinuity_type])
+            discontinuity_details.append(
+                [epoch_index, timeaxis[epoch_index], discontinuity_type]
+            )
         epoch_index += 1
         # message("Progress: %f%%\r"%(epoch_index*100./len(timeaxis)))
 
     # Print the result
     # changed discontinuity_timestamps to discontinuity details May 5 2022
     if len(discontinuity_details) != 0:
         message("The data is discontinuous!")
@@ -322,16 +354,22 @@
     while ii_index < ki_index - 1:
         # Repetition condition :if the successive time stamp is less than or
         # equal to the present, delete the row.
         if (time[ii_index + 1] - time[ii_index]) <= -0.1 * delta_t:
             # Set flag to 1 if repetition condition is met.
             rep_row_index = 1
             if verbose == "yes":
-                message("found a repeating row at %d, time %f\n" % (ii_index + 1, time[ii_index + 1]))
-                message("timei: %f timef %f\n" % (time[ii_index], time[ii_index + 1]))
+                message(
+                    "found a repeating row at %d, time %f\n"
+                    % (ii_index + 1, time[ii_index + 1])
+                )
+                message(
+                    "timei: %f timef %f\n"
+                    % (time[ii_index], time[ii_index + 1])
+                )
             # ci = ci+1
             # Delete the entire row
             time = np.delete(time, ii_index + 1)
             # data = np.delete(data,ii_index,1)
             # data = [np.delete(item,ii_index+1) for item in data]
             data = np.delete(data, ii_index + 1, axis)
             # Append the deleted index to the bookkeeping array
@@ -428,22 +466,31 @@
     # rowcounter
     counter = 0
 
     # Iterate over rows
     while ii_index < ki_index - 1:
         # Repetition condition :if the successive time stamp is less than or
         # equal to the present, delete the row.
-        if (time[ii_index + 1] == time[ii_index]) or (time[ii_index] - time[ii_index + 1]) >= toldt * delta_t:
+        if (time[ii_index + 1] == time[ii_index]) or (
+            time[ii_index] - time[ii_index + 1]
+        ) >= toldt * delta_t:
             # if time[ii_index]-time[ii_index+1]<=0.01*delta_t:
             # 		 message("Error!!",message_verbosity=0)
             # Set flag to 1 if repetition condition is met.
             rep_row_index = 1
             counter += 1
-            message("found a repeating row at %d, time %f\n" % (ii_index + 1, time[ii_index + 1]), message_verbosity=3)
-            message("timei: %f timef %f\n" % (time[ii_index], time[ii_index + 1]), message_verbosity=3)
+            message(
+                "found a repeating row at %d, time %f\n"
+                % (ii_index + 1, time[ii_index + 1]),
+                message_verbosity=3,
+            )
+            message(
+                "timei: %f timef %f\n" % (time[ii_index], time[ii_index + 1]),
+                message_verbosity=3,
+            )
             # ci = ci+1
             # Delete the entire row
             time = np.delete(time, ii_index + 1, 0)
             # data = np.delete(data,ii_index,1)
             # data = [np.delete(item,ii_index+1) for item in data]
             data = np.delete(data, ii_index + 1, axis)
             # Append the deleted index to the bookkeeping array
@@ -463,15 +510,18 @@
     else:
         message("No points removed\n", message_verbosity=2)
         # message("++++++++++++++++++++++++++++++++++++++++++++++++++++++\n")
     # Return the "cleaned" data matrix
     cleaned_data = data
 
     if bridge and iscontinuous(cleaned_data)[-1] >= 2:
-        message("The data will be interpolated to bridge the gaps", message_verbosity=2)
+        message(
+            "The data will be interpolated to bridge the gaps",
+            message_verbosity=2,
+        )
 
         # from scipy import interpolate
 
         # Interpolate the data to fill in the discontinuities
         t_final = time[-1]
         t_initial = time[0]
 
@@ -618,34 +668,43 @@
                 recentered_timestamp - original_timestamp
             ) >= toldt * delta_t:
                 # if recentered_timestamp-original_timestamp<=0.01*delta_t:
                 # 		 message("Error!!",message_verbosity=0)
                 repetition = 1
                 discont_type = repetition
                 message(
-                    "Repetitive rows found at index: %d,timestamp: %f" % (index, original_timestamp),
+                    "Repetitive rows found at index: %d,timestamp: %f"
+                    % (index, original_timestamp),
                     message_verbosity=3,
                 )
                 message(
-                    "Repetition at timestamp original: %f correct %f\n" % (original_timestamp, recentered_timestamp),
+                    "Repetition at timestamp original: %f correct %f\n"
+                    % (original_timestamp, recentered_timestamp),
                     message_verbosity=3,
                 )
                 repetition_counter += 1
             # Missing rows
-            if (original_timestamp - recentered_timestamp) >= (1.0 + toldt) * delta_t:
+            if (original_timestamp - recentered_timestamp) >= (
+                1.0 + toldt
+            ) * delta_t:
                 discont = 2
                 discont_type = discont
                 message(
-                    "Jump discountinuity in data found at index:%d,timestamp:%f" % (index, original_timestamp),
+                    "Jump discountinuity in data found at index:%d,timestamp:%f"
+                    % (index, original_timestamp),
                     message_verbosity=2,
                 )
                 message("delta_t=%f" % delta_t, message_verbosity=1)
                 message(
                     "Jump at timestamp original: %f correct %f\n Dt = %f"
-                    % (original_timestamp, recentered_timestamp, (original_timestamp - recentered_timestamp) / delta_t),
+                    % (
+                        original_timestamp,
+                        recentered_timestamp,
+                        (original_timestamp - recentered_timestamp) / delta_t,
+                    ),
                     message_verbosity=1,
                 )
                 discont_counter += 1
             # message("timei: %f timef %f\n"%(timeaxis[index-1],timeaxis[index]),message_verbosity=3)
 
             # discont_type=repetition+discont
             discont_type_details.append([index, discont_type])
@@ -655,21 +714,33 @@
         index += 1
         # message("Progress: %f%%\r"%(epoch_index*100./len(timeaxis)))
     # discont_type=(repetition+discont)
     # Print the result
     if discont_type:
         message("The data is not clean!", message_verbosity=1)
         global_discont_type = repetition + discont
-        message("Discontinuity type:", global_discont_type, message_verbosity=1)
+        message(
+            "Discontinuity type:", global_discont_type, message_verbosity=1
+        )
         if global_discont_type == 1:
-            message("The data has repetitive rows at %d locations" % repetition_counter, message_verbosity=1)
+            message(
+                "The data has repetitive rows at %d locations"
+                % repetition_counter,
+                message_verbosity=1,
+            )
         elif global_discont_type == 2:
-            message("The data has %d discontinuities" % discont_counter, message_verbosity=1)
+            message(
+                "The data has %d discontinuities" % discont_counter,
+                message_verbosity=1,
+            )
         else:
-            message("The data has repetitive rows and is discontinious", message_verbosity=1)
+            message(
+                "The data has repetitive rows and is discontinious",
+                message_verbosity=1,
+            )
 
         discontinuity_details = [discont_type_details, global_discont_type]
     else:
         message("Data is continuous", message_verbosity=2)
         discontinuity_details = [[0, 0], 0]
     # Return the details of discontinuity
 
@@ -720,22 +791,31 @@
     # rowcounter
     counter = 0
 
     # Iterate over rows
     while ii_index < ki_index - 1:
         # Repetition condition :if the successive time stamp is less than or
         # equal to the present, delete the row.
-        if (time[ii_index + 1] == time[ii_index]) or (time[ii_index] - time[ii_index + 1]) >= toldt * delta_t:
+        if (time[ii_index + 1] == time[ii_index]) or (
+            time[ii_index] - time[ii_index + 1]
+        ) >= toldt * delta_t:
             # if time[ii_index]-time[ii_index+1]<=0.01*delta_t:
             # 		 message("Error!!",message_verbosity=0)
             # Set flag to 1 if repetition condition is met.
             rep_row_index = 1
             counter += 1
-            message("found a repeating row at %d, time %f\n" % (ii_index + 1, time[ii_index + 1]), message_verbosity=3)
-            message("timei: %f timef %f\n" % (time[ii_index], time[ii_index + 1]), message_verbosity=3)
+            message(
+                "found a repeating row at %d, time %f\n"
+                % (ii_index + 1, time[ii_index + 1]),
+                message_verbosity=3,
+            )
+            message(
+                "timei: %f timef %f\n" % (time[ii_index], time[ii_index + 1]),
+                message_verbosity=3,
+            )
             # ci = ci+1
             # Delete the entire row
             time = np.delete(time, ii_index + 1, 0)
             # data = np.delete(data,ii_index,1)
             # data = [np.delete(item,ii_index+1) for item in data]
             data = np.delete(data, ii_index + 1, axis)
             # Append the deleted index to the bookkeeping array
```

### Comparing `waveformtools-2023.6.5/waveformtools/simulations.py` & `waveformtools-2023.7.14/waveformtools/simulations.py`

 * *Files 5% similar despite different names*

```diff
@@ -273,87 +273,122 @@
         self.ref_multipoles = ref_multipoles
         self.indjn = indjn
         self.NP_1d = NP_1d
 
     @property
     def data_duration(self):
         """Compute and return the data duration of the simulations."""
-        return {alias: self.data_length[alias] * self.delta_t[alias] for alias in self.aliases}
+        return {
+            alias: self.data_length[alias] * self.delta_t[alias]
+            for alias in self.aliases
+        }
 
     @property
     def comm_data_duration(self):
         """Compute and return the duration of
         the common data (multipole and Bhdiag/distance)
         of the simulations."""
-        return {alias: self.comm_data_length[alias] * self.delta_t[alias] for alias in self.aliases}
+        return {
+            alias: self.comm_data_length[alias] * self.delta_t[alias]
+            for alias in self.aliases
+        }
 
     @property
     def pm_data_duration(self):
         """Compute and return the duration
         of post-merger data present in the simulations."""
-        return {alias: self.data_duration[alias] - self.merger_time[alias] for alias in self.aliases}
+        return {
+            alias: self.data_duration[alias] - self.merger_time[alias]
+            for alias in self.aliases
+        }
 
     @property
     def pm_data_length(self):
         """Compute and return the post merger
         data length avaialable for all simulations."""
-        return {alias: self.data_length[alias] - self.merger_ind[alias] for alias in self.aliases}
+        return {
+            alias: self.data_length[alias] - self.merger_ind[alias]
+            for alias in self.aliases
+        }
 
     @property
     def merger_distance(self):
         """Compute and return the distance
         at the merger index of the simulations."""
         merger_dist = {}
         for alias in self.aliases:
             try:
-                merger_dist.update({alias: self.distance[alias][self.merger_ind[alias]]})
+                merger_dist.update(
+                    {alias: self.distance[alias][self.merger_ind[alias]]}
+                )
             except IndexError:
                 if (self.merger_ind[alias] - len(self.distance[alias])) == 1:
-                    merger_dist.update({alias: self.distance[alias][self.merger_ind[alias] - 1]})
+                    merger_dist.update(
+                        {
+                            alias: self.distance[alias][
+                                self.merger_ind[alias] - 1
+                            ]
+                        }
+                    )
                 else:
-                    message("%s :Distance upto merger not defined. Setting final value" % alias)
+                    message(
+                        "%s :Distance upto merger not defined. Setting final value"
+                        % alias
+                    )
                     merger_dist.update({alias: self.distance[alias][-1]})
         return merger_dist
 
     @property
     def true_merger_distance(self):
         """Compute and return the true
         (i.e. non-normalized) distance at merger for the simulations."""
-        return {alias: self.dinit[alias] * self.merger_distance[alias] for alias in self.aliases}
+        return {
+            alias: self.dinit[alias] * self.merger_distance[alias]
+            for alias in self.aliases
+        }
 
     @property
     def sampling_f(self):
         """Compute and return the sampling frequency of the simulations."""
         return {alias: 1.0 / self.delta_t[alias] for alias in self.aliases}
 
     @property
     def merger_time(self):
         """Compute and return the
         cctk_time stamp at the merger
         for the simulations."""
-        return {alias: self.merger_ind[alias] * self.delta_t[alias] for alias in self.aliases}
+        return {
+            alias: self.merger_ind[alias] * self.delta_t[alias]
+            for alias in self.aliases
+        }
 
     @property
     def massratio(self):
         """Compute and return the massratio of the simulations."""
-        return {alias: self.mass2[alias] / self.mass1[alias] for alias in self.aliases}
+        return {
+            alias: self.mass2[alias] / self.mass1[alias]
+            for alias in self.aliases
+        }
 
     @property
     def chirpmass(self):
         """Compute and return the chirp mass of the simulations."""
         return {
             alias: ((self.mass1[alias] * self.mass2[alias]) ** (3.0 / 5))
             / (self.mass1[alias] + self.mass2[alias]) ** (1.0 / 5)
             for alias in self.aliases
         }
 
     @property
     def totalmass(self):
         """Compute and return the total mass of the simulations."""
-        return {alias: self.mass1[alias] + self.mass2[alias] for alias in self.aliases}
+        return {
+            alias: self.mass1[alias] + self.mass2[alias]
+            for alias in self.aliases
+        }
 
     def calc_junkend(self, tjn=200.0):
         """Compute the indices and the starting distances
         of the system at timestamp t = 200.
 
         Parameters
         ----------
@@ -427,17 +462,27 @@
                 self.comm_data_length[alias] = ml_length
                 self.distance[alias] = self.distance[alias][:ml_length]
             message(item.shape)
             log_mult.update(
                 {
                     alias: [
                         item[: self.comm_data_length[alias], 0],
-                        np.log(np.absolute(-item[: self.comm_data_length[alias], 1])),
-                        np.log(np.absolute(-item[: self.comm_data_length[alias], 2])),
-                        np.log(np.absolute(-item[self.merger_ind[alias] :, 3])),
+                        np.log(
+                            np.absolute(
+                                -item[: self.comm_data_length[alias], 1]
+                            )
+                        ),
+                        np.log(
+                            np.absolute(
+                                -item[: self.comm_data_length[alias], 2]
+                            )
+                        ),
+                        np.log(
+                            np.absolute(-item[self.merger_ind[alias] :, 3])
+                        ),
                     ]
                 }
             )
         self.log_multipoles = log_mult
 
     def calc_delta_multipoles(self):
         """Compute and return the delta multipoles (w.r.t. reference (l=2) multipoles)"""
@@ -467,15 +512,22 @@
             Ml22_ref = np.mean(Ml22[30:100])
             Ml32_ref = np.mean(Ml32[-100:])
             dMl12 = Ml12 - Ml12_ref
             dMl22 = Ml22 - Ml22_ref
             dMl32 = Ml32 - Ml32_ref
 
             log_deltmult.update(
-                {alias: [time, np.log(np.absolute(-dMl12)), np.log(np.absolute(-dMl22)), np.log(np.absolute(-dMl32))]}
+                {
+                    alias: [
+                        time,
+                        np.log(np.absolute(-dMl12)),
+                        np.log(np.absolute(-dMl22)),
+                        np.log(np.absolute(-dMl32)),
+                    ]
+                }
             )
 
         self.log_deltamultipoles = log_deltmult
 
     def calc_log_multipoles2(self):
         """Compute and assign the natural logarithm of the (l=2) multipoles to sim.log_multipoles of the simulations."""
         log_mult = {}
@@ -526,15 +578,17 @@
             Ml12_ref = np.mean(Ml12[30:100])
             Ml22_ref = np.mean(Ml22[30:100])
             Ml32_ref = np.mean(Ml32[-100:])
             dMl12 = Ml12 - Ml12_ref
             dMl22 = Ml22 - Ml22_ref
             dMl32 = Ml32 - Ml32_ref
 
-            log_deltmult.update({alias: [time, np.log(-dMl12), np.log(-dMl22), np.log(dMl32)]})
+            log_deltmult.update(
+                {alias: [time, np.log(-dMl12), np.log(-dMl22), np.log(dMl32)]}
+            )
 
         self.log_deltamultipoles2 = log_deltmult
 
     def load_data(self):
         """Load data of the simulations.
 
         Notes
@@ -599,15 +653,18 @@
             # Loop over simulations.
 
             message(self.aliases[sim_index])
             message("------------------")
 
             # Load the qlm_multipole moment data.
             file0 = np.genfromtxt(
-                self.ROOTDIR + sim1[sim_index] + self.data_dir + "quasilocalmeasures-qlm_multipole_moments..asc"
+                self.ROOTDIR
+                + sim1[sim_index]
+                + self.data_dir
+                + "quasilocalmeasures-qlm_multipole_moments..asc"
             )
 
             # Assign the timeaxis.
             cctk_time = file0[:, 8]
 
             # Assign the multipole data lengths to a list.
             ml_data_length.append(len(cctk_time))
@@ -708,15 +765,17 @@
 
             try:
                 # Try to find the jump location of the horizon mass1 data.
                 merger_one = np.where(np.diff(M1_one_all) > 0.1)[0]
 
             except BaseException:
                 merger_one = len(M1_one_all)
-                message("Mass1 has no jumps. Merger has probably not happened. Reverting to data length.")
+                message(
+                    "Mass1 has no jumps. Merger has probably not happened. Reverting to data length."
+                )
 
             message("Merger index (through jump in mass1):", merger_one)
 
             if merger_one_a.any() and merger_one.any():
                 # If both indices have been found, select the least of the two
                 # as merger index.
                 merger_one = min(merger_one_a[0], merger_one[0])
@@ -733,15 +792,17 @@
                 message("No merger data exists")
                 merger_one = -1
 
             else:
                 # If both indices are not equal, declare inconsistency but
                 # accept the result from either.
 
-                message("Merger index inconsistency found. Mergertime may not be correct")
+                message(
+                    "Merger index inconsistency found. Mergertime may not be correct"
+                )
 
                 try:
                     # First try with non-zero mass3 index.
                     merger_one = merger_one[0]
                     message("Merger time set from Mass3")
                 except BaseException:
                     # Else assign from mass1 jump.
@@ -781,38 +842,54 @@
             # Gather the mass and spin multipoles together.
             all_mass_multipoles_one.append([amm1, amm2, amm3])
             all_spin_multipoles_one.append([asm1, asm2, asm3])
 
             # message(len(cctk_time))
 
             # Gather the l=2 mass multipoles.
-            multipoles_one.append(np.array([cctk_time, Ml12_one, Ml22_one, Ml32_one]))
+            multipoles_one.append(
+                np.array([cctk_time, Ml12_one, Ml22_one, Ml32_one])
+            )
 
             # Gather the masses.
             masses_one.append([M1_one, M2_one, M3_one])
             masses_one_all.append([M1_one_all, M2_one_all, M3_one_all])
 
             ###################################################################
             # II . Load the distance data.
             # Compute the distance using the coordinate positions in BHdiagnostics files.
             ###################################################################
-            temp0 = np.genfromtxt(self.ROOTDIR + sim1[sim_index] + self.data_dir + "BH_diagnostics.ah1.gp")
-            temp1 = np.genfromtxt(self.ROOTDIR + sim1[sim_index] + self.data_dir + "BH_diagnostics.ah2.gp")
+            temp0 = np.genfromtxt(
+                self.ROOTDIR
+                + sim1[sim_index]
+                + self.data_dir
+                + "BH_diagnostics.ah1.gp"
+            )
+            temp1 = np.genfromtxt(
+                self.ROOTDIR
+                + sim1[sim_index]
+                + self.data_dir
+                + "BH_diagnostics.ah2.gp"
+            )
 
             t_coord_0 = temp0[:, 1]
             x_coord_0_locs = temp0[:, 2]
             y_coord_0_locs = temp0[:, 3]
 
             message("Coord len", len(t_coord_0))
             t_coord_1 = temp1[:, 1]
             x_coord_1_locs = temp1[:, 2]
             y_coord_1_locs = temp1[:, 3]
 
-            temp0 = np.transpose(np.array([t_coord_0, x_coord_0_locs, y_coord_0_locs]))
-            temp1 = np.transpose(np.array([t_coord_1, x_coord_1_locs, y_coord_1_locs]))
+            temp0 = np.transpose(
+                np.array([t_coord_0, x_coord_0_locs, y_coord_0_locs])
+            )
+            temp1 = np.transpose(
+                np.array([t_coord_1, x_coord_1_locs, y_coord_1_locs])
+            )
 
             message("Dist shapes", temp0.shape, temp1.shape)
             # check for data continuity.
             # Load data.
             data0 = temp0
             data1 = temp1
 
@@ -831,23 +908,30 @@
 
             # message('Time step',delta_t)
 
             # Retrieve merger index.
             mergerind = ind_merger_one[sim_index]
 
             # Update the merger time list.
-            merger_time_one.append(ind_merger_one[sim_index] * delta_t_one[sim_index])
+            merger_time_one.append(
+                ind_merger_one[sim_index] * delta_t_one[sim_index]
+            )
 
             # Find the shorter data. BHdiag1,2 or multipole data.
             act_len = min(shape0[0], shape1[0], ml_data_length[sim_index])
 
             # If BHdiag 1 and 2 are equal in length and equal to multipole
             # length:
-            if shape0[0] == shape1[0] and shape0[0] == ml_data_length[sim_index]:
-                message("BH_data length is consistent with multipole data length")
+            if (
+                shape0[0] == shape1[0]
+                and shape0[0] == ml_data_length[sim_index]
+            ):
+                message(
+                    "BH_data length is consistent with multipole data length"
+                )
 
             # If the shortest data length is different from multipole length.
             if act_len == shape0[0] or act_len == shape1[0]:
                 message("BH_diagnostics data is shorter")
 
             # If multipole data is shorter.
             else:
@@ -861,31 +945,41 @@
             # act_shape_one.append()#
             # act_shape_one.append(min(shape1[0],shape2[0]))
             # message(temp0.shape,temp1.shape)
 
             # Try to load BHdiag3 file if present.
             try:
                 # Try to load the BH_diagnostics file for BH3.
-                temp2 = np.genfromtxt(self.ROOTDIR + sim1[sim_index] + self.data_dir + "BH_diagnostics.ah3.gp")[
-                    :, np.r_[1, 2, 3]
-                ]
+                temp2 = np.genfromtxt(
+                    self.ROOTDIR
+                    + sim1[sim_index]
+                    + self.data_dir
+                    + "BH_diagnostics.ah3.gp"
+                )[:, np.r_[1, 2, 3]]
 
                 # If merger index is not found from masses set using BH_diag3.
 
                 # If the merger_ind from masses is greater than the BHdiag3
                 # data length.
 
                 if mergerind * delta_t >= int(temp2[0, 0]):
                     merger_time_one[sim_index] = temp2[0, 0]
                     mergerind = int(temp2[0, 0] / delta_t)
                     ind_merger_one[sim_index] = mergerind
-                    message("Merger time acquired from BHdiag3", mergerind * delta_t)
-                    message("Merger index has been updated with info from BHdiag3")
+                    message(
+                        "Merger time acquired from BHdiag3",
+                        mergerind * delta_t,
+                    )
+                    message(
+                        "Merger index has been updated with info from BHdiag3"
+                    )
             except BaseException:
-                message("Merger time acquired from masses", mergerind * delta_t)
+                message(
+                    "Merger time acquired from masses", mergerind * delta_t
+                )
 
             message("Merger index", mergerind)
 
             # FInd shape of data.
             shape0 = temp0.shape
             shape1 = temp1.shape
 
@@ -954,15 +1048,20 @@
             d0_one.append(d0_sim)
             d_sim = d_sim / d0_sim
             # d_one.append(np.sqrt((temp0[:act_shape_one[sim_index],1]-temp1[:act_shape_one[sim_index],1])**2
             # + (temp0[:act_shape_one[sim_index],2]-temp1[:act_shape_one[sim_index],2])**2))
             d_one.append([t_coord_0, d_sim])
             message(
                 "ml_timeaxis_length: %d, Multipole data length: %d, BHdiag length: %d, Distance length: %d"
-                % (len(timeaxis_one[sim_index]), ml_data_length[sim_index], shape1[0], len(d_one[sim_index]))
+                % (
+                    len(timeaxis_one[sim_index]),
+                    ml_data_length[sim_index],
+                    shape1[0],
+                    len(d_one[sim_index]),
+                )
             )
             dist_data_length.append(len(d_sim))
 
         # multipoles = np.array(multipoles)
         # Convert the acquired data lists into numpy arrays.
         masses_one = np.array(masses_one)
         M1_one = np.array(M1_one)
@@ -982,29 +1081,49 @@
         # d_one.shape
 
         # Plot the distance
         # message('multipoles length',len(multipoles_one))
 
         # Assign data to sim variables.
         for sim_index in range(0, len(self.aliases)):
-            self.multipoles.update({self.aliases[sim_index]: multipoles_one[sim_index]})
-            self.mass_multipoles.update({self.aliases[sim_index]: all_mass_multipoles_one[sim_index]})
-            self.spin_multipoles.update({self.aliases[sim_index]: all_spin_multipoles_one[sim_index]})
-            self.timeaxis.update({self.aliases[sim_index]: timeaxis_one[sim_index]})
+            self.multipoles.update(
+                {self.aliases[sim_index]: multipoles_one[sim_index]}
+            )
+            self.mass_multipoles.update(
+                {self.aliases[sim_index]: all_mass_multipoles_one[sim_index]}
+            )
+            self.spin_multipoles.update(
+                {self.aliases[sim_index]: all_spin_multipoles_one[sim_index]}
+            )
+            self.timeaxis.update(
+                {self.aliases[sim_index]: timeaxis_one[sim_index]}
+            )
             self.mass1.update({self.aliases[sim_index]: M1_one[sim_index]})
             self.mass2.update({self.aliases[sim_index]: M2_one[sim_index]})
             self.mass3.update({self.aliases[sim_index]: M3_one[sim_index]})
-            self.delta_t.update({self.aliases[sim_index]: delta_t_one[sim_index]})
+            self.delta_t.update(
+                {self.aliases[sim_index]: delta_t_one[sim_index]}
+            )
             self.distance.update({self.aliases[sim_index]: d_one[sim_index]})
-            self.merger_ind.update({self.aliases[sim_index]: ind_merger_one[sim_index]})
-            self.actmerger_time.update({self.aliases[sim_index]: merger_time_one[sim_index]})
+            self.merger_ind.update(
+                {self.aliases[sim_index]: ind_merger_one[sim_index]}
+            )
+            self.actmerger_time.update(
+                {self.aliases[sim_index]: merger_time_one[sim_index]}
+            )
             self.dinit.update({self.aliases[sim_index]: d0_one[sim_index]})
-            self.data_length.update({self.aliases[sim_index]: ml_data_length[sim_index]})
-            self.comm_data_length.update({self.aliases[sim_index]: act_shape_one[sim_index]})
-            self.dist_data_length.update({self.aliases[sim_index]: dist_data_length[sim_index]})
+            self.data_length.update(
+                {self.aliases[sim_index]: ml_data_length[sim_index]}
+            )
+            self.comm_data_length.update(
+                {self.aliases[sim_index]: act_shape_one[sim_index]}
+            )
+            self.dist_data_length.update(
+                {self.aliases[sim_index]: dist_data_length[sim_index]}
+            )
         # message(self.multipoles)
 
         # Resize the multipoles data if merger index was updated from BHdiag3.
         self._resize_multipoles()
         # Reverse the BH1 and BH2 data if BH mass2>mass1.
         self._ifreversal()
 
@@ -1029,15 +1148,18 @@
     def _resize_multipoles(self):
         """Private method to resize the (l=2) multipole data. Useful when merger index was updated from BHdiag3."""
         for alias in self.aliases:
             # Loop over simulations.
             # message(alias)
             # self.timeaxis[alias] = [item[:self.dist_data_length[alias]] for item in self.timeaxis[alias]]
             # Resize the lengths of the data.
-            self.multipoles[alias] = [item[: self.dist_data_length[alias]] for item in self.multipoles[alias]]
+            self.multipoles[alias] = [
+                item[: self.dist_data_length[alias]]
+                for item in self.multipoles[alias]
+            ]
             # self.data_length.update({alias : len(self.multipoles[alias][0])})
             # self.mass_multipoles[alias] = [item[:self.dist_data_length[alias] for item in self.mass_multipoles[alias]]]
             # self.spin_multipoles[alias] = [item[:self.dist_data_length[alias]
             # for item in self.spin_multipoles[alias]]]
 
     def _ifreversal(self):
         """Private method to reverse the (l=2) multipole data if mass2>mass1.
@@ -1056,26 +1178,42 @@
             # Loop over simulations.
             message("Check for puncture reversal, %s" % alias)
             if alias != "q1a0_a" and alias != "q1a0_b":
                 # Condition for reversal decision.
                 if self.mass1[alias] < self.mass2[alias]:
                     # Toggle the flag.
                     flag = 1
-                    message("**************************************************")
-                    message("BH 1 and 2 reversal found!!! \n Reversing data...")
-                    message("**************************************************")
-                    message("original mass1:%f, mass2: %f" % (self.mass1[alias], self.mass2[alias]))
+                    message(
+                        "**************************************************"
+                    )
+                    message(
+                        "BH 1 and 2 reversal found!!! \n Reversing data..."
+                    )
+                    message(
+                        "**************************************************"
+                    )
+                    message(
+                        "original mass1:%f, mass2: %f"
+                        % (self.mass1[alias], self.mass2[alias])
+                    )
                     # Reverse the data.
-                    self.mass1[alias], self.mass2[alias] = self.mass2[alias], self.mass1[alias]
+                    self.mass1[alias], self.mass2[alias] = (
+                        self.mass2[alias],
+                        self.mass1[alias],
+                    )
                     # Unpack the multipoles data.
-                    time, multipole1, multipole2, multipole3 = self.multipoles[alias]
+                    time, multipole1, multipole2, multipole3 = self.multipoles[
+                        alias
+                    ]
                     # Reverse the multipole data.
                     multipole1, multipole2 = multipole2, multipole1
                     # Repack the data.
-                    self.multipoles[alias] = np.array([time, multipole1, multipole2, multipole3])
+                    self.multipoles[alias] = np.array(
+                        [time, multipole1, multipole2, multipole3]
+                    )
             if not flag:
                 message("Data O.K.")
             return 1.0
 
     def load_strain(self, start_index=0):
         """Method to load the shear data of simulations."""
 
@@ -1159,33 +1297,61 @@
 
             # Load the plus and cross polarized strain data.
             hpdat = self.strain[alias][1]
             hxdat = self.strain[alias][2]
             # Load the time stepping.
             delta_t = self.delta_t[alias]
             # Extract and update the amplitude and phases.
-            self.strain_phase.update({alias: (xtract_cphase(hpdat, hxdat, delta_t=delta_t, to_plot="yes"))})
+            self.strain_phase.update(
+                {
+                    alias: (
+                        xtract_cphase(
+                            hpdat, hxdat, delta_t=delta_t, to_plot="yes"
+                        )
+                    )
+                }
+            )
             self.strain_amplitude.update({alias: xtract_camp(hpdat, hxdat)})
-            self.strain_frequency.update({alias: np.diff(self.strain_phase[alias]) / delta_t})
+            self.strain_frequency.update(
+                {alias: np.diff(self.strain_phase[alias]) / delta_t}
+            )
         return 1
 
     def ret_horizon_radii(self):
         """Retrieve the radius of the common horizon at the time of formation."""
 
         # Dictionary to hold the areal radii of the horizons.
         self.areal_radii = {}
         for alias in self.aliases:
             # Loop over simulations.
 
             # Load the BHdiagnostics file to load the radius.
-            ar_rad0 = np.genfromtxt(self.ROOTDIR + alias + "/" + self.data_dir + "BH_diagnostics.ah1.gp")[:, 27]
-            ar_rad1 = np.genfromtxt(self.ROOTDIR + alias + "/" + self.data_dir + "BH_diagnostics.ah2.gp")[:, 27]
+            ar_rad0 = np.genfromtxt(
+                self.ROOTDIR
+                + alias
+                + "/"
+                + self.data_dir
+                + "BH_diagnostics.ah1.gp"
+            )[:, 27]
+            ar_rad1 = np.genfromtxt(
+                self.ROOTDIR
+                + alias
+                + "/"
+                + self.data_dir
+                + "BH_diagnostics.ah2.gp"
+            )[:, 27]
             ar_rad2 = 1.75
             try:
-                ar_rad2 = np.genfromtxt(self.ROOTDIR + alias + "/" + self.data_dir + "BH_diagnostics.ah3.gp")[:, 27]
+                ar_rad2 = np.genfromtxt(
+                    self.ROOTDIR
+                    + alias
+                    + "/"
+                    + self.data_dir
+                    + "BH_diagnostics.ah3.gp"
+                )[:, 27]
             except BaseException:
                 message("No BHdiagnostics 3 file found for %s" % alias)
 
             # Load the data for this simulation in to a dictionary.
             self.areal_radii.update({alias: [ar_rad0, ar_rad1, ar_rad2]})
 
         return 1
@@ -1222,18 +1388,26 @@
 
             # Masses of the horizons
             m1 = self.mass1[alias]
             m2 = self.mass2[alias]
             # M = m1 + m2
 
             flag = 1
-            bh1 = np.genfromtxt(self._get_file_path_from_str(string="*.ah1.gp", alias=alias))
-            bh2 = np.genfromtxt(self._get_file_path_from_str(string="*.ah2.gp", alias=alias))
+            bh1 = np.genfromtxt(
+                self._get_file_path_from_str(string="*.ah1.gp", alias=alias)
+            )
+            bh2 = np.genfromtxt(
+                self._get_file_path_from_str(string="*.ah2.gp", alias=alias)
+            )
             try:
-                bh3 = np.genfromtxt(self._get_file_path_from_str(string="*.ah3.gp", alias=alias))
+                bh3 = np.genfromtxt(
+                    self._get_file_path_from_str(
+                        string="*.ah3.gp", alias=alias
+                    )
+                )
             except Exception as excep:
                 message("BH3 file not found!", excep)
                 flag = -1
 
             # Read co-ordinates.
 
             bhd1_time = bh1[:, 1]
@@ -1317,17 +1491,23 @@
             total_mass = mass1 + mass2
 
             # End time
             max_len = min(self.merger_ind[alias], len(bh1_time), len(bh2_time))
 
             # CoM location
             T_com = bh1_time[:max_len]
-            X_com = (mass1 * bh1_x[:max_len] + mass2 * bh2_x[:max_len]) / (total_mass)
-            Y_com = (mass1 * bh1_y[:max_len] + mass2 * bh2_y[:max_len]) / (total_mass)
-            Z_com = (mass1 * bh1_z[:max_len] + mass2 * bh2_z[:max_len]) / (total_mass)
+            X_com = (mass1 * bh1_x[:max_len] + mass2 * bh2_x[:max_len]) / (
+                total_mass
+            )
+            Y_com = (mass1 * bh1_y[:max_len] + mass2 * bh2_y[:max_len]) / (
+                total_mass
+            )
+            Z_com = (mass1 * bh1_z[:max_len] + mass2 * bh2_z[:max_len]) / (
+                total_mass
+            )
 
             self.CoM_locations.update({alias: [T_com, X_com, Y_com, Z_com]})
 
     def get_CoM_mean_motion(self, alias=None):
         """Get the mean motion of the CoM.
 
         Parameters
@@ -1348,15 +1528,19 @@
                            A dictionary containing the
                            mean CoM velocity array.
 
         """
         CoM_motion_params = {}
         # Aliases to run over.
 
-        from waveformtools.CoM import X_com_moments, compute_com_alpha, compute_com_beta
+        from waveformtools.CoM import (
+            X_com_moments,
+            compute_com_alpha,
+            compute_com_beta,
+        )
 
         if not alias:
             list_of_aliases = self.aliases
 
         else:
             list_of_aliases = [alias]
 
@@ -1369,16 +1553,20 @@
                 taxis, X_com, Y_com, Z_com = self.CoM_locations[alias]
 
             all_coords = [X_com, Y_com, Z_com]
 
             zeroth_moments = X_com_moments(taxis, all_coords, 0)
             first_moments = X_com_moments(taxis, all_coords, 1)
 
-            Xcom_0 = np.array([zeroth_moments[label][0] for label in zeroth_moments.keys()])
-            Xcom_1 = np.array([first_moments[label][0] for label in zeroth_moments.keys()])
+            Xcom_0 = np.array(
+                [zeroth_moments[label][0] for label in zeroth_moments.keys()]
+            )
+            Xcom_1 = np.array(
+                [first_moments[label][0] for label in zeroth_moments.keys()]
+            )
 
             ti = taxis[0]
             tf = taxis[-1]
 
             alpha = compute_com_alpha(ti, tf, Xcom_0, Xcom_1)
             beta = compute_com_beta(ti, tf, Xcom_0, Xcom_1)
 
@@ -1439,29 +1627,42 @@
 
         np_data_alias_dict = {}
 
         for alias in self.aliases:
             if source == "qlm":
                 file_string = f"{self.data_dir}quasilocalmeasures-qlm_newman_penrose..asc"
             elif source == "ih":
-                file_string = f"{self.data_dir}isolatedhorizon-ih_newman_penrose..asc"
+                file_string = (
+                    f"{self.data_dir}isolatedhorizon-ih_newman_penrose..asc"
+                )
 
-            full_file_path = self._get_file_path_from_str(alias, string=file_string)
+            full_file_path = self._get_file_path_from_str(
+                alias, string=file_string
+            )
 
             with open(full_file_path, "r") as file:
                 for line_index in range(15):
                     fline = next(file)
                     # message(fline)
                     str_match = re.search(f"\d\d:qlm_np{np_qty}", fline)
                     # message(str_match)
                     if str_match is not None:
                         start_col = int(str_match[0][:2])
                         # message(start_col)
                         break
 
             NP_all_data = np.genfromtxt(full_file_path)[
-                :, np.r_[8, start_col - 1, start_col, start_col + 1, start_col + 2, start_col + 3, start_col + 4]
+                :,
+                np.r_[
+                    8,
+                    start_col - 1,
+                    start_col,
+                    start_col + 1,
+                    start_col + 2,
+                    start_col + 3,
+                    start_col + 4,
+                ],
             ]
 
             np_data_alias_dict.update({alias: NP_all_data})
 
         self.NP_1d.update({np_qty: np_data_alias_dict})
```

### Comparing `waveformtools-2023.6.5/waveformtools/spherical.py` & `waveformtools-2023.7.14/waveformtools/spherical.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 ##################################
 # Imports
 #################################
 
 import numpy as np
 
 
-def decompose_in_SWSHs(waveform, gridinfo, spin_weight=-2, ell_max=8, emm_list="all"):
+def decompose_in_SWSHs(
+    waveform, gridinfo, spin_weight=-2, ell_max=8, emm_list="all"
+):
     """Decompose a given function on a sphere in Spin Weighted Spherical Harmonics
 
     Parameters
     ----------
 
     waveform:		list
                     A list that contains as its items the waveform
@@ -111,23 +113,27 @@
             for emm_index in range(len(emm_list)):
                 # Decompose into seperate m modes.
 
                 # m value.
                 emm_val = int(emm_list[emm_index])
 
                 # Spin weighted spherical harmonic function at (theta, phi)
-                Ybasis_fun = Yslm_vec(spin_weight, ell_index, emm_val, theta, phi)
+                Ybasis_fun = Yslm_vec(
+                    spin_weight, ell_index, emm_val, theta, phi
+                )
 
                 # Integrate to obtain the multipole of order l.
 
                 # Integration for real and imaginary parts of the data separately.
                 # Integrate the function
 
                 # Using quad
-                multipole_emm = quad_on_sphere(integrand_ij * Ybasis_fun * darea, gridinfo)
+                multipole_emm = quad_on_sphere(
+                    integrand_ij * Ybasis_fun * darea, gridinfo
+                )
                 # multipole_emm	 =	 np.sum(integrand_ij * Ybasis_fun * darea)
 
                 multipoles_ell.update({emm_val: multipole_emm})
             multipoles_all.update({ell_index: multipoles_ell})
 
         # Return the computed multipole.
         return multipoles_all
@@ -180,30 +186,36 @@
     theta_first_integral_errs = []
     # Step 1: integrate along the theta direction
     for phi_index in range(gridinfo.nphi):
         # Interpolate the integrand.
 
         integrand_phi = integrand[:, phi_index]
 
-        integrand_phi_interp_func = interp1d(theta_1d, integrand_phi, kind=kind)
+        integrand_phi_interp_func = interp1d(
+            theta_1d, integrand_phi, kind=kind
+        )
 
         # Integrate on the phi plane
-        integral_phi_vals, integral_phi_errs = quad(integrand_phi_interp_func, 0, np.pi)
+        integral_phi_vals, integral_phi_errs = quad(
+            integrand_phi_interp_func, 0, np.pi
+        )
 
         theta_first_integral_vals.append(integral_phi_vals)
         theta_first_integral_errs.append(integral_phi_errs)
 
     # Step 2: integrate along the phi direction
 
     # Interpolate the integrand.
 
     integrand_theta = theta_first_integral_vals
 
     integrand_theta_interp_func = interp1d(phi_1d, integrand_theta, kind=kind)
 
     # Integrate on the theta plane
-    final_integral, semi_final_errs = quad(integrand_theta_interp_func, 0, 2 * np.pi)
+    final_integral, semi_final_errs = quad(
+        integrand_theta_interp_func, 0, 2 * np.pi
+    )
 
     # Get final errors
     final_errs = semi_final_errs + np.sum(np.array(theta_first_integral_errs))
 
     return final_integral, final_errs
```

### Comparing `waveformtools-2023.6.5/waveformtools/transforms.py` & `waveformtools-2023.7.14/waveformtools/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,33 +200,44 @@
         factor = (-1) ** ell
         theta = np.pi - theta
         phi += np.pi
 
     abs_spin_weight = abs(spin_weight)
 
     for aar in range(ell - abs_spin_weight + 1):
-        if (aar + abs_spin_weight - emm) < 0 or (ell - aar - abs_spin_weight) < 0:
+        if (aar + abs_spin_weight - emm) < 0 or (
+            ell - aar - abs_spin_weight
+        ) < 0:
             message(f"Skippin r {aar}", message_verbosity=3)
             continue
         else:
             Sum += (
                 sp.binomial(ell - abs_spin_weight, aar)
-                * sp.binomial(ell + abs_spin_weight, aar + abs_spin_weight - emm)
+                * sp.binomial(
+                    ell + abs_spin_weight, aar + abs_spin_weight - emm
+                )
                 * np.power((-1), (ell - aar - abs_spin_weight))
                 * np.exp(1j * emm * phi)
-                / np.power(np.tan(theta / 2), (2 * aar + abs_spin_weight - emm))
+                / np.power(
+                    np.tan(theta / 2), (2 * aar + abs_spin_weight - emm)
+                )
             )
 
     Sum = complex(Sum)
     Yslm = (-1) ** emm * (
         np.sqrt(
             fact(ell + emm)
             * fact(ell - emm)
             * (2 * ell + 1)
-            / (4 * np.pi * fact(ell + abs_spin_weight) * fact(ell - abs_spin_weight))
+            / (
+                4
+                * np.pi
+                * fact(ell + abs_spin_weight)
+                * fact(ell - abs_spin_weight)
+            )
         )
         * np.sin(theta / 2) ** (2 * ell)
         * Sum
     )
 
     return factor * Yslm
 
@@ -274,33 +285,42 @@
         phi_grid += np.pi
 
     abs_spin_weight = abs(spin_weight)
 
     for aar in range(0, ell - abs_spin_weight + 1):
         subterm = 0
 
-        if (aar + abs_spin_weight - emm) < 0 or (ell - aar - abs_spin_weight) < 0:
+        if (aar + abs_spin_weight - emm) < 0 or (
+            ell - aar - abs_spin_weight
+        ) < 0:
             message(f"Skipping r {aar}", message_verbosity=3)
             continue
         else:
             term1 = comb(ell - abs_spin_weight, aar)
             term2 = comb(ell + abs_spin_weight, aar + abs_spin_weight - emm)
             term3 = np.power(float(-1), (ell - aar - abs_spin_weight))
             term4 = np.exp(1j * emm * phi_grid)
-            term5 = np.power(np.tan(theta_grid / 2), (-2 * aar - abs_spin_weight + emm))
+            term5 = np.power(
+                np.tan(theta_grid / 2), (-2 * aar - abs_spin_weight + emm)
+            )
             subterm = term1 * term2 * term3 * term4 * term5
 
             Sum += subterm
 
     Yslmv = float(-1) ** emm * (
         np.sqrt(
             fact(ell + emm)
             * fact(ell - emm)
             * (2 * ell + 1)
-            / (4 * np.pi * fact(ell + abs_spin_weight) * fact(ell - abs_spin_weight))
+            / (
+                4
+                * np.pi
+                * fact(ell + abs_spin_weight)
+                * fact(ell - abs_spin_weight)
+            )
         )
         * np.sin(theta_grid / 2) ** (2 * ell)
         * Sum
     )
 
     return factor * Yslmv
 
@@ -338,15 +358,17 @@
 
     Yslm_expr = Yslm_prec_sym(spin_weight, ell, emm)
 
     if spin_weight < 0:
         theta = np.pi - theta
         phi = np.pi + phi
 
-    return Yslm_expr.evalf(prec, subs={th: sp.Float(f"{theta}"), ph: sp.Float(f"{phi}")})
+    return Yslm_expr.evalf(
+        prec, subs={th: sp.Float(f"{theta}"), ph: sp.Float(f"{phi}")}
+    )
 
 
 def Yslm_prec_sym(spin_weight, ell, emm):
     """Spin-weighted spherical harmonics precise, symbolic computation for deferred evaluations.
        Is dependent on variables th: theta and ph:phi.
     Parameters
     ----------
@@ -382,15 +404,17 @@
     # To get negative spin weight SWSH
     # in terms of positive spin weight
     factor = 1
     if spin_weight < 0:
         factor = sp.Pow(-1, ell)
 
     for aar in range(ell - abs_spin_weight + 1):
-        if (aar + abs_spin_weight - emm) < 0 or (ell - aar - abs_spin_weight) < 0:
+        if (aar + abs_spin_weight - emm) < 0 or (
+            ell - aar - abs_spin_weight
+        ) < 0:
             # message('Continuing')
             continue
         else:
             # message('r, l, s, m', r, l, s, m)
             # a1 = sp.binomial(ell - spin_weight, aar)
             # message(a1)
             # a2 = sp.binomial(ell + spin_weight, aar + spin_weight - emm)
@@ -398,26 +422,33 @@
             # a3 = sp.exp(1j * emm * phi)
             # message(a3)
             # a4 = sp.tan(theta / 2)
             # message(a4)
 
             Sum += (
                 sp.binomial(ell - abs_spin_weight, aar)
-                * sp.binomial(ell + abs_spin_weight, aar + abs_spin_weight - emm)
+                * sp.binomial(
+                    ell + abs_spin_weight, aar + abs_spin_weight - emm
+                )
                 * sp.Pow((-1), (ell - aar - abs_spin_weight))
                 * sp.exp(sp.I * emm * ph)
                 * sp.Pow(sp.cot(th / 2), (2 * aar + abs_spin_weight - emm))
             )
 
     Yslm_expr = sp.Pow(-1, emm) * (
         sp.sqrt(
             fact(ell + emm)
             * fact(ell - emm)
             * (2 * ell + 1)
-            / (4 * sp.pi * fact(ell + abs_spin_weight) * fact(ell - abs_spin_weight))
+            / (
+                4
+                * sp.pi
+                * fact(ell + abs_spin_weight)
+                * fact(ell - abs_spin_weight)
+            )
         )
         * sp.Pow(sp.sin(th / 2), (2 * ell))
         * Sum
     )
 
     Yslm_expr = factor * sp.simplify(Yslm_expr)
```

### Comparing `waveformtools-2023.6.5/waveformtools/waveformtools.py` & `waveformtools-2023.7.14/waveformtools/waveformtools.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,19 @@
 
 # matplotlib.use('Agg')
 from matplotlib import pyplot as plt
 from termcolor import colored
 
 
 def message(
-    *args, message_verbosity=2, print_verbosity=config.print_verbosity, log_verbosity=config.log_verbosity, **kwargs
+    *args,
+    message_verbosity=2,
+    print_verbosity=config.print_verbosity,
+    log_verbosity=config.log_verbosity,
+    **kwargs,
 ):
     """The print function with verbosity levels and logging facility.
 
     Notes
     -----
     Verbosity choices:
 
@@ -90,15 +94,17 @@
             os.mkdir("logs")
 
         with open("logs/" + tstamp + ".log", "a") as log_file:
             if message_verbosity == -1:
                 for line in traceback.format_stack():
                     log_file.write(line.strip())
             log_file.write("\n")
-            log_file.write("{}:{}\t{}".format(caller.filename, caller.lineno, *args))
+            log_file.write(
+                "{}:{}\t{}".format(caller.filename, caller.lineno, *args)
+            )
             log_file.write("\n")
     return 1
 
 
 def mode(a_list):
     """Find the mode of a list
 
@@ -245,25 +251,30 @@
                             The differentiated 1d data
                             as pycbc TimeSeries"""
 
     if not delta_t:
         try:
             delta_t = data.delta_t
         except BaseException:
-            message("Input is not a TimeSeries. Please supply gridspacing as delta_t", message_verbosity=0)
+            message(
+                "Input is not a TimeSeries. Please supply gridspacing as delta_t",
+                message_verbosity=0,
+            )
 
     dydx = np.diff((np.array(data))) / delta_t
 
     if TS is True:
         dydx = pycbc.types.timeseries.TimeSeries(dydx, delta_t)
 
     return dydx
 
 
-def integrate_first_order(data, t_start=None, t_end=None, delta_t=None, to_taper=False, TS=False):
+def integrate_first_order(
+    data, t_start=None, t_end=None, delta_t=None, to_taper=False, TS=False
+):
     """Integrate a timeseries using first order method.
 
     Notes
     -----
     Capabilities
 
     Simple Euler integrator, option to taper the ends.
@@ -289,15 +300,17 @@
             # Find sampling time_step
             delta_t = data.delta_t
             data_time = data.sample_times
             t_start_dat, t_end_dat = data_time[0], data_time[-1]
 
         except BaseException:
             message(
-                "Input is not a TimeSeries." "Please input a pycbc TimeSeries" "or supply gridspacing as delta_t",
+                "Input is not a TimeSeries."
+                "Please input a pycbc TimeSeries"
+                "or supply gridspacing as delta_t",
                 message_verbosity=0,
             )
     else:
         t_start_dat = 0
         t_end_dat = len(data) * delta_t
 
     if not t_start:
@@ -331,15 +344,17 @@
 
     data = np.array(data)
 
     for i in range(1, end_index - start_index):
         integdat[i] = integdat[i - 1] + (data[start_index + i - 1]) * delta_t
 
     if TS is True:
-        integdat = pycbc.types.timeseries.TimeSeries(integdat, delta_t, epoch=t_start)
+        integdat = pycbc.types.timeseries.TimeSeries(
+            integdat, delta_t, epoch=t_start
+        )
 
     return integdat
 
 
 def compute_frequencies(t_coal, t_val, chirp_mass):
     """Compute the Newtonian instantaneous frequency
     of strain waveform from coalescence time and
@@ -354,15 +369,19 @@
     chirp_mass :    float
                                     The chirpmass.
 
     Returns
     -------
     freqs : float
                     The instantaneous frequency of the strain waveform."""
-    freqs = (1.0 / (np.pi * chirp_mass)) * (5.0 / 256) ** (3.0 / 8) * (chirp_mass / (t_coal - t_val)) ** (3.0 / 8)
+    freqs = (
+        (1.0 / (np.pi * chirp_mass))
+        * (5.0 / 256) ** (3.0 / 8)
+        * (chirp_mass / (t_coal - t_val)) ** (3.0 / 8)
+    )
 
     return freqs
 
 
 def totalmass(mass_ratio, chirp_mass):
     """Find total mass from mass ratio and chirpmass.
 
@@ -375,15 +394,17 @@
 
     Returns
     -------
     total_mass :    float
                                     The total mass of the system.
     """
 
-    return (chirp_mass * (1.0 + mass_ratio) ** (6.0 / 5)) / mass_ratio ** (3.0 / 5)
+    return (chirp_mass * (1.0 + mass_ratio) ** (6.0 / 5)) / mass_ratio ** (
+        3.0 / 5
+    )
 
 
 def massratio(chirp_mass):
     """Compute the mass ratio from chirpmass. Assumes total mass to be 1.
 
     Parameters
     ----------
@@ -392,15 +413,17 @@
 
     Returns
     -------
     mass_ratio :    float
                                     The Mass ratio of the system
     """
     mass_ratio = (
-        chirp_mass ** (1.0 / 3) - 2.0 * chirp_mass**2.0 - np.sqrt(chirp_mass ** (2.0 / 3) - 4.0 * chirp_mass ** (7.0 / 3))
+        chirp_mass ** (1.0 / 3)
+        - 2.0 * chirp_mass**2.0
+        - np.sqrt(chirp_mass ** (2.0 / 3) - 4.0 * chirp_mass ** (7.0 / 3))
     ) / (2.0 * chirp_mass**2.0)
 
     return mass_ratio
 
 
 # Defining function for calculating Chirpmass from a2
 
@@ -504,24 +527,32 @@
         lflag = "ab"
 
     # If data_a < data_b
     elif len(data_a) < len(data_b):
         # add zeros to data_a when a is smaller
         lflag = "a"
         zers = len(data_b) - len(data_a)
-        signala = np.transpose(np.concatenate((np.transpose(data_a), np.transpose(np.zeros([zers])))))
+        signala = np.transpose(
+            np.concatenate(
+                (np.transpose(data_a), np.transpose(np.zeros([zers])))
+            )
+        )
         # signala = pycbc.types.timeseries.TimeSeries(signala, delta_t)
         # return pycbc.types.timeseries.TimeSeries(signalb,delta_t),lflag
     # If data_b < data_a
     else:
         # message("Error!")
         # add zeros to b when b is smaller
         lflag = "b"
         zers = len(data_a) - len(data_b)
-        signalb = np.transpose(np.concatenate((np.transpose(data_b), np.transpose(np.zeros([zers])))))
+        signalb = np.transpose(
+            np.concatenate(
+                (np.transpose(data_b), np.transpose(np.zeros([zers])))
+            )
+        )
         # signalb = pycbc.types.timeseries.TimeSeries(signalb, delta_t)
         # return pycbc.types.timeseries.TimeSeries(signala,delta_t),lflag
 
     # Returns a list containing the length equalized arrays and the flag.
     if not is_ts:
         signala = np.array(signala)
         signalb = np.array(signalb)
@@ -558,15 +589,17 @@
             delta_t = signala.delta_t
 
         except AttributeError:
             try:
                 delta_t = signalb.delta_t
             except BaseException:
                 message(
-                    "Input is not a TimeSeries." "Please supply a pycbc TimeSeries object " "or the gridspacing as delta_t",
+                    "Input is not a TimeSeries."
+                    "Please supply a pycbc TimeSeries object "
+                    "or the gridspacing as delta_t",
                     message_verbosity=0,
                 )
 
     # Ensure data is numpy array.
     signalb = np.array(data_b)
     # Taper waveform A.
     signala = np.array(taper(data_a, delta_t))
@@ -721,15 +754,15 @@
         message("The time array:%s" % time, message_verbosity=3)
     else:
         time = data
 
     # Index of ros to delete
     dind = []
 
-    discontinuities = iscontinuous_new(time)
+    discontinuities = iscontinuous(time)
 
     repetition = bool(discontinuities["repetitions"][0])
 
     if repetition:
         rep_rows = discontinuities["repetitions"][1]
 
         data = np.delete(data, rep_rows)
@@ -771,35 +804,42 @@
 
     s1, l = data.shape
 
     from scipy.stats import mode
 
     delta_t = mode(np.diff(time))[0][0]
 
-    discontinuities = iscontinuous_new(time)
+    discontinuities = iscontinuous(time)
 
     gaps = bool(discontinuties["gaps"][0])
 
     if gaps:
         gap_rows = discontinuoties["gaps"][1]
-        message("The data will be interpolated to bridge the gaps", message_verbosity=2)
+        message(
+            "The data will be interpolated to bridge the gaps",
+            message_verbosity=2,
+        )
 
         # Interpolate the data to fill in the discontinuities
         t_final = time[-1]
         t_initial = time[0]
 
         proper_timeaxis = np.arange(t_initial, t_final, delta_t)
 
         interp_data = []
         interp_data.append(proper_timeaxis)
 
-        from scipy.interpolate import InterpolatedUnivariateSpline as interpolator
+        from scipy.interpolate import (
+            InterpolatedUnivariateSpline as interpolator,
+        )
 
         for index in range(1, s1):
-            interp_data.append(interpolator(time, data[index, :], k=k)(proper_timeaxis))
+            interp_data.append(
+                interpolator(time, data[index, :], k=k)(proper_timeaxis)
+            )
 
         cleaned_data = np.array(interp_data)
         message("The data has been interpolated", message_verbosity=3)
     else:
         message("No jumps found in the data", message_verbosity=2)
 
     return cleaned_data
@@ -889,37 +929,44 @@
     """
 
     if is_ts:
         if not delta_t:
             try:
                 delta_t = hdat.delta_t
             except BaseException:
-                message("Input is not a TimeSeries. Please supply gridspacing as delta_t", message_verbosity=0)
+                message(
+                    "Input is not a TimeSeries. Please supply gridspacing as delta_t",
+                    message_verbosity=0,
+                )
 
     if ind > 0:
         # ind>0 case for shifting array to the right
         # message hdat
         # Length of the data
         # l = len(hdat)
         # Array holding zeroes to be appended
         zeros = np.zeros([ind])
         # The shifted array
-        shifted_wf = np.transpose(np.concatenate((np.transpose(zeros), np.transpose(hdat))))[:-ind]
+        shifted_wf = np.transpose(
+            np.concatenate((np.transpose(zeros), np.transpose(hdat)))
+        )[:-ind]
         # message msig
         # message msig[:-ind]
         # Return the clipped, shifted timeseries
 
     elif ind < 0:
         # ind <0 case for shifting array to the left
         # Length of the data
         # l = len(hdat)
         # Array holding zeroes to be appended
         zeros = np.zeros([ind])
         # The shifted array
-        shifted_wf = np.transpose(np.concatenate((np.transpose(hdat), np.transpose(zeros))))[ind:]
+        shifted_wf = np.transpose(
+            np.concatenate((np.transpose(hdat), np.transpose(zeros)))
+        )[ind:]
         # message msig
         # message msig[:-ind]
         # Return a timeseries
 
     else:
         shifted_wf = hdat
 
@@ -1108,15 +1155,17 @@
                             A list containing complex amplitude
                             (list) and phase (list).
     """
 
     return xtract_camp(tsdata_1, tsdata_2), xtract_cphase(tsdata_1, tsdata_2)
 
 
-def get_waveform_angular_frequency(waveform, delta_t, timeaxis=None, method="FD"):
+def get_waveform_angular_frequency(
+    waveform, delta_t, timeaxis=None, method="FD"
+):
     """Get the angular frequency of the waveform given
     the complex waveform time step. The phase is
     extracted and is differentiated using one of
     the available methods to compute the angular
     frequency.
 
     Parameters
@@ -1325,21 +1374,27 @@
                              The pair of indices denoting the start
                              and end points of an array
     """
 
     try:
         start_index = np.where(np.array(data) != 0)[0][0]
     except BaseException:
-        message(colored("Warning! Start index not found!!", "red"), message_verbosity=1)
+        message(
+            colored("Warning! Start index not found!!", "red"),
+            message_verbosity=1,
+        )
         start_index = 0
 
     try:
         end_index = np.where(np.array(data) != 0)[0][-1] + 1
     except BaseException:
-        message(colored("Warning! End index not found!!", "red"), message_verbosity=1)
+        message(
+            colored("Warning! End index not found!!", "red"),
+            message_verbosity=1,
+        )
         end_index = 0
     return start_index, end_index
 
 
 def apxstartend(data, tol=1e-5):
     """Identify the Approximate start and endpoints of the data.
 
@@ -1386,19 +1441,23 @@
            The waveform data as list or numpy array or pycbc timeseries.
     zeros : int
             The number of zeros to be added.
 
     Returns
     -------
     data : 1darray
-           data with `zeros` number of zeros concatenated 
+           data with `zeros` number of zeros concatenated
            at the end as numpy 1d array
     """
 
-    return np.transpose(np.concatenate((np.transpose(np.array(data)), np.transpose(np.zeros([zeros])))))
+    return np.transpose(
+        np.concatenate(
+            (np.transpose(np.array(data)), np.transpose(np.zeros([zeros])))
+        )
+    )
 
 
 def removezeros(data, delta_t):
     """Remove zeros from the input waveform from either sides.
     Similar to startend but return the truncated array.
 
     Parameters
@@ -1407,30 +1466,36 @@
            The input waveform.
     delta_t : float, optional
               The time stepping.
 
     Returns
     -------
     short_ts : a list
-               A list containing waveforms with zeros 
+               A list containing waveforms with zeros
                removed on either sides,
                the start and end indices in the format [short_ts, [start_index, end_index]]
 
     """
 
     # Assign the timestep. Real and imaginary parts are assumed to have same
     # timestep.
     if not delta_t:
         try:
             delta_t = data.delta_t
         except BaseException:
-            message("Input is not a TimeSeries." " Please supply gridspacing as delta_t", message_verbosity=0)
+            message(
+                "Input is not a TimeSeries."
+                " Please supply gridspacing as delta_t",
+                message_verbosity=0,
+            )
 
     starti, endi = startend(data)
-    ret_data = pycbc.types.timeseries.TimeSeries(np.array(data)[starti:endi], delta_t)
+    ret_data = pycbc.types.timeseries.TimeSeries(
+        np.array(data)[starti:endi], delta_t
+    )
 
     short_ts = [ret_data, [starti, endi]]
 
     return short_ts
 
 
 def shorten(tsdata, start, end, delta_t=None):
@@ -1457,22 +1522,30 @@
     # are assumed to have same
 
     # timestep.
     if not delta_t:
         try:
             delta_t = tsdata.delta_t
         except BaseException:
-            message("Input is not a TimeSeries." "Please supply gridspacing as delta_t", message_verbosity=0)
+            message(
+                "Input is not a TimeSeries."
+                "Please supply gridspacing as delta_t",
+                message_verbosity=0,
+            )
 
-    short_ts = pycbc.types.timeseries.TimeSeries(np.array(tsdata)[start:end], delta_t)
+    short_ts = pycbc.types.timeseries.TimeSeries(
+        np.array(tsdata)[start:end], delta_t
+    )
 
     return short_ts
 
 
-def taper_tanh(waveform, time_axis=None, delta_t=None, duration=10, sides="both"):
+def taper_tanh(
+    waveform, time_axis=None, delta_t=None, duration=10, sides="both"
+):
     """
     Taper a waveform with a :math:`tanh` function
     at either ends
 
     Parameters
     ----------
     waveform : 1d array
@@ -1532,33 +1605,46 @@
     # end_axis   = np.linspace(1, -1, nend_points)
 
     # norm_time_axis = time_axis/max(time_axis)
 
     # n_delta_t = delta_t/data_len
 
     # from scipy.interpolate import interpolate
-    waveform_widened = np.concatenate((np.zeros([nstart_points]), waveform, np.zeros([nend_points - 1])))
+    waveform_widened = np.concatenate(
+        (np.zeros([nstart_points]), waveform, np.zeros([nend_points - 1]))
+    )
     new_time_axis = np.linspace(
-        time_axis[0] - nstart_points * delta_t, time_axis[-1] + nend_points * delta_t, len(waveform_widened)
+        time_axis[0] - nstart_points * delta_t,
+        time_axis[-1] + nend_points * delta_t,
+        len(waveform_widened),
     )
 
-    start_win = (np.tanh(3 * (new_time_axis - duration / 2) / (duration / 2)) + 1) / 2
-    end_win = (np.tanh(3 * (-new_time_axis + (tfinal - duration / 2)) / (duration / 2)) + 1) / 2
+    start_win = (
+        np.tanh(3 * (new_time_axis - duration / 2) / (duration / 2)) + 1
+    ) / 2
+    end_win = (
+        np.tanh(
+            3 * (-new_time_axis + (tfinal - duration / 2)) / (duration / 2)
+        )
+        + 1
+    ) / 2
 
     # plt.scatter(new_time_axis, waveform_widened, s=1)
     # plt.show()
 
     if sides == "both":
         tapered_waveform = start_win * end_win * waveform_widened
     elif sides == "beg":
         tapered_waveform = start_win * waveform_widened
     elif sides == "end":
         tapered_waveform = end_win * waveform_widened
     else:
-        message("Please specify valid sides argument. Sides can be beg, end or both.")
+        message(
+            "Please specify valid sides argument. Sides can be beg, end or both."
+        )
 
     # plt.scatter(new_time_axis, tapered_waveform, s=1)
     # plt.show()
 
     return new_time_axis, tapered_waveform
 
 
@@ -1605,17 +1691,21 @@
 
     # Append the zeros
     tapered_data = np.array(tapered_data)
 
     # Pad ends with extra zeros
     zeros = np.zeros([zeros])
     # Prepend with z zeros
-    tapered_data = np.transpose(np.concatenate((np.transpose(zeros), np.transpose(tapered_data))))
+    tapered_data = np.transpose(
+        np.concatenate((np.transpose(zeros), np.transpose(tapered_data)))
+    )
     # Append with extra zeros
-    tapered_data = np.transpose(np.concatenate((np.transpose(tapered_data), np.transpose(zeros))))
+    tapered_data = np.transpose(
+        np.concatenate((np.transpose(tapered_data), np.transpose(zeros)))
+    )
 
     # Convert back to timeseries if the input was a time series.
     tapered_data = pycbc.types.timeseries.TimeSeries(tapered_data, delta_t)
 
     # Return the timeseries
     return tapered_data
 
@@ -1691,47 +1781,53 @@
     if not delta_t:
         try:
             delta_t = wvp.delta_t
         except AttributeError:
             try:
                 delta_t = wvc.delta_t
             except BaseException:
-                message("Input is not a TimeSeries." "Please supply gridspacing as delta_t", message_verbosity=0)
+                message(
+                    "Input is not a TimeSeries."
+                    "Please supply gridspacing as delta_t",
+                    message_verbosity=0,
+                )
 
     datap = np.array(wvp)
     datac = np.array(wvc)
 
     # Assign the complex amplitude
     amp = np.power(datap, 2) + np.power(datac, 2)
     # Find the location of the max amplitude
     ind = np.where(amp == np.max(amp))[0][0]
     # Calculate the epoch
     tlim = [-ind * delta_t, (len(datap) - ind) * delta_t]
     # Returns the centered wvp and wvc if wvc was provided else returns just
     # the former.
 
     if flag == 1:
-        centered_wf = pycbc.types.timeseries.TimeSeries(datap, delta_t, epoch=tlim[0])
+        centered_wf = pycbc.types.timeseries.TimeSeries(
+            datap, delta_t, epoch=tlim[0]
+        )
     else:
         centered_wf = (
             pycbc.types.timeseries.TimeSeries(datap, delta_t, epoch=tlim[0]),
             pycbc.types.timeseries.TimeSeries(datac, delta_t, epoch=tlim[0]),
         )
 
     return centered_wf
 
 
 def get_centered_taxis(time_ax, amps):
-    """Get the time axis of the waveform centered 
+    """Get the time axis of the waveform centered
     at its maximum absolute amplitude.
 
     Parameters
     ----------
     time_ax : 1d array
-              The 1d array containg the original 
+              The 1d array containg the original
               (uncentered)time axis of the wveform.
 
     amps : 1d array
            The amplitude of the waveform.
 
     Returns
     -------
@@ -1775,16 +1871,17 @@
     plt.xlabel("xdata")
     plt.ylabel("f(x)")
     if save != "no":
         plt.savefig(save + ".pdf")
     plt.show()
     return 1
 
+
 def coalignwfs(tsdata1, tsdata2, delta_t=None):
-    """Coalign two timeseries. Wrapper and modification around 
+    """Coalign two timeseries. Wrapper and modification around
     pycbc functions with some additional functionalities.
 
     Parameters
     ----------
     tsdata1, tsdata2 : list, 1d array or a pycbc TimeSeries
                        The two data vectors as 1d lists or
                        numpy arrays or pycbc TimeSeries
@@ -1819,15 +1916,19 @@
     if not delta_t:
         try:
             delta_t = tsdata1.delta_t
         except AttributeError:
             try:
                 delta_t = tsdata2.delta_t
             except BaseException:
-                message("Input is not a TimeSeries." "Please supply gridspacing as delta_t", message_verbosity=0)
+                message(
+                    "Input is not a TimeSeries."
+                    "Please supply gridspacing as delta_t",
+                    message_verbosity=0,
+                )
 
     tsdata1, tsdata2, _ = lengtheq(tsdata1, tsdata2, delta_t, is_ts=True)
 
     # Calculate complex SNR using pycbc function. Note: This complex SNR is
     # actually the complex SNR * norm of the timeseries.
     csnr = pycbc.filter.matchedfilter.matched_filter(tsdata1, tsdata2)
     # Find the absolute value of the complex SNR timeseries
@@ -1922,34 +2023,48 @@
 
     # match,shift=pycbc.filter.matchedfilter.match(tsdata1,tsdata2)
 
     # Normalize the waveforms
     norm1 = norm(np.array(tsdata1[start:end]))
     norm2 = norm(np.array(tsdata2[start:end]))
 
-    tsdata1_cropped = pycbc.types.timeseries.TimeSeries(np.array(tsdata1[start:end]) / norm1, delta_t)
-    tsdata2_cropped = pycbc.types.timeseries.TimeSeries(np.array(tsdata2[start:end]) / norm2, delta_t)
+    tsdata1_cropped = pycbc.types.timeseries.TimeSeries(
+        np.array(tsdata1[start:end]) / norm1, delta_t
+    )
+    tsdata2_cropped = pycbc.types.timeseries.TimeSeries(
+        np.array(tsdata2[start:end]) / norm2, delta_t
+    )
 
-    max_match, max_shift = pycbc.filter.matchedfilter.match(tsdata1_cropped, tsdata2_cropped)
+    max_match, max_shift = pycbc.filter.matchedfilter.match(
+        tsdata1_cropped, tsdata2_cropped
+    )
 
-    tsdata1 = pycbc.types.timeseries.TimeSeries(np.array(tsdata1) / norm1, delta_t)
-    tsdata2 = pycbc.types.timeseries.TimeSeries(np.array(tsdata2) / norm2, delta_t)
+    tsdata1 = pycbc.types.timeseries.TimeSeries(
+        np.array(tsdata1) / norm1, delta_t
+    )
+    tsdata2 = pycbc.types.timeseries.TimeSeries(
+        np.array(tsdata2) / norm2, delta_t
+    )
 
     # Calculate complex SNR using pycbc function. Note: This complex SNR is
     # actually the complex SNR * norm of the timeseries.
     csnr = pycbc.filter.matchedfilter.matched_filter(tsdata1, tsdata2)
 
     # Find the absolute value of the complex SNR timeseries
     acsnr = np.array(np.abs(csnr))
     # message(acsnr,np.max(acsnr))
 
     # Find the location of the maximum element in acsnr
     maxloc = (np.where(acsnr == np.max(acsnr)))[0][0]
     mmatch = np.amax(acsnr)
-    message(f"Max location is {maxloc}," f"match is {mmatch}" f"max shift is {max_shift}")
+    message(
+        f"Max location is {maxloc},"
+        f"match is {mmatch}"
+        f"max shift is {max_shift}"
+    )
 
     # Shift the waveform 1 in time using maxloc
     tsdata1 = shiftmatched(tsdata1, maxloc, delta_t, is_ts=True)
 
     # Phase shift ( rotate) the waveform 1 by multipying
     # the frequency series of waveform 1 with the phase
     # of the max element in acsnr
@@ -1959,19 +2074,27 @@
     rotation = csnr[maxloc] / np.absolute(csnr[maxloc])
 
     # Rotate and take the inverse Fourier transform
     ctsdata1 = (rotation * tsdata1.to_frequencyseries()).to_timeseries()
 
     # Recenter waveform 0 and assign the timeaxis of waveform 0 to waveform1
     ctsdata1, dummy = center(ctsdata1, ctsdata1)
-    tsdata2 = pycbc.types.timeseries.TimeSeries(np.array(tsdata2), tsdata2.delta_t, epoch=ctsdata1.sample_times[0])
+    tsdata2 = pycbc.types.timeseries.TimeSeries(
+        np.array(tsdata2), tsdata2.delta_t, epoch=ctsdata1.sample_times[0]
+    )
 
     # Return the normalized, time and phase shifted waveform 1 to coalign with
     # 2 and waveform 2.
-    aligned_waveforms = {"wf1": ctsdata1, "wf2": tsdata2, "norms": [norm1, norm2], "shift": maxloc, "match": max_match}
+    aligned_waveforms = {
+        "wf1": ctsdata1,
+        "wf2": tsdata2,
+        "norms": [norm1, norm2],
+        "shift": maxloc,
+        "match": max_match,
+    }
 
     return aligned_waveforms
 
 
 def resample_wfs(both_time_axes, both_waveforms, delta_t="auto", Plot=False):
     """Resample the waveform pairs.
 
@@ -2067,15 +2190,15 @@
     Returns
     -------
     match_details : dict
                                                                                                                                                                                                                                                                     A dictionary containing the
                                                                                                                                                                                                                                                                     i). match coeffient
                                                                                                                                                                                                                                                                     ii). time_shift
                                                                                                                                                                                                                                                                     iii). phase shift in radians
-                                                                                                                                                                                                                                                                    iv). normalized, resampled, waveforms 
+                                                                                                                                                                                                                                                                    iv). normalized, resampled, waveforms
                            and their time-axes.
 
     Note
     ----
     The shifts give by how much the first waveform has to be shifted to match with the second.
 
     """
@@ -2096,15 +2219,17 @@
 
             # delta_t = min(delta_t_A, delta_t_B)
         elif delta_t == "A":
             delta_t = delta_t_A
         elif delta_t == "B":
             delta_t = delta_t_B
         else:
-            raise ValueError(f"Did not understand speification for delta_t {delta_t}")
+            raise ValueError(
+                f"Did not understand speification for delta_t {delta_t}"
+            )
 
     # message(type(time_axis1), type(time_axis2))
     # message(time_axis1-time_axis2)
     # message(time_axis1==time_axis2)
 
     # Don't interpolate if the time axis are identical
     Interp = True
@@ -2120,15 +2245,17 @@
             # tsorted = sorted(time_axis1)
             # delta_t = tsorted[0] - tsorted[1]
 
             # delta_t = mode(np.diff(time_axis1))
 
     if Interp is True:
         message("Interpolating time axis")
-        time_axis, wf1, wf2 = resample_wfs(all_time_axes, all_waveforms, delta_t)
+        time_axis, wf1, wf2 = resample_wfs(
+            all_time_axes, all_waveforms, delta_t
+        )
         # message(time_axis, wf1, wf2)
 
     from waveformtools.transforms import compute_fft, compute_ifft
 
     # The Fspace waveforms
     faxis, wf1_tilde = compute_fft(wf1, delta_t)
     _, wf2_tilde = compute_fft(wf2, delta_t)
@@ -2146,17 +2273,21 @@
     # max_snr = np.amax(Acsnr)
 
     Tshift_rec = (len(time_axis) - Tshift_rec_index) * delta_t
     # Phase shift
     Pshift_rec = csnr[Tshift_rec_index] / np.absolute(csnr[Tshift_rec_index])
     Pshift_rec_rad = np.log(Pshift_rec) / (1j)
 
-    message("-----------------------------------\n Shift information for waveform 2 against 1 \n")
+    message(
+        "-----------------------------------\n Shift information for waveform 2 against 1 \n"
+    )
     message(f"Recovered Time shift: {Tshift_rec}")
-    message(f"Recovered Phase shift: {Pshift_rec}, {Pshift_rec_rad} in radians")
+    message(
+        f"Recovered Phase shift: {Pshift_rec}, {Pshift_rec_rad} in radians"
+    )
     message("-----------------------------------")
 
     # Apply the time shift to the second waveform
 
     if Tshift_rec_index != 0:
         wf2_Trec = roll(wf2, Tshift_rec_index)
     else:
@@ -2176,15 +2307,17 @@
 
     norm1 = np.sqrt(np.sum(wf1 * np.conjugate(wf1)))
     norm2 = np.sqrt(np.sum(wf2_TPrec * np.conjugate(wf2_TPrec)))
 
     waveform1_aligned = wf1 / norm1
     waveform2_aligned = wf2_TPrec / norm2
 
-    match_score = np.sum(waveform1_aligned * np.conjugate(waveform2_aligned))  # max_snr/(norm1*norm2)
+    match_score = np.sum(
+        waveform1_aligned * np.conjugate(waveform2_aligned)
+    )  # max_snr/(norm1*norm2)
 
     match_details = {
         "match_score": match_score,
         "time_shift": Tshift_rec,
         "phase_shift": Pshift_rec_rad,
         "time": time_axis,
         "aligned_waveforms": [waveform1_aligned, waveform2_aligned],
@@ -2302,15 +2435,17 @@
 
     mlen = min(len(wf1_aligned_cropped), len(wf2_shifted))
 
     waveform1_aligned = wf1_aligned_cropped[:mlen] / norm1
     waveform2_aligned = wf2_shifted[:mlen] / norm2
 
     aligned_time_axis = aligned_time_axis[:mlen]
-    match_score = np.dot(wf1_aligned_cropped[:mlen], np.conjugate(wf2_shifted[:mlen])) / (norm1 * norm2)
+    match_score = np.dot(
+        wf1_aligned_cropped[:mlen], np.conjugate(wf2_shifted[:mlen])
+    ) / (norm1 * norm2)
 
     match_details = {
         "match_score": match_score,
         "time_shift": shift * delta_t,
         "phase_shift": phase_shift,
         "time": aligned_time_axis,
         "aligned_waveforms": [waveform1_aligned, waveform2_aligned],
@@ -2321,69 +2456,86 @@
 
 def simplematch_wfs_old(waveforms, delta_t=None):
     """Simple match the given waveforms. Does not clip the waveforms at either ends.
 
     Parameters
     ----------
     waveforms : list
-				A list of pairs [waveform A, waveform B] of waveforms.
+                                A list of pairs [waveform A, waveform B] of waveforms.
     delta_t : float, optional
-			  The time stepping.
+                          The time stepping.
 
     Notes
     -----
     The time stepping delta_t is the same for each pair of waveforms in the list.
 
     Returns
     -------
     match : list
             A list of dicts [{ Aligned waveforms} ,
-							{match score (float), shift (number)}]
-			containing the match information for all the input waveform pairs.
+                                                        {match score (float), shift (number)}]
+                        containing the match information for all the input waveform pairs.
     """
 
     match = []
     # Iterate over (signal,template) pairs in waveforms
     for waveformdat in waveforms:
         # Carryout the match
         if not delta_t:
             try:
                 delta_t = waveformdat[0].delta_t
             except BaseException:
-                message("Waveform is not a pycbc TimeSeries." "Please provide the gridspacing delt")
+                message(
+                    "Waveform is not a pycbc TimeSeries."
+                    "Please provide the gridspacing delt"
+                )
                 sys.exit(0)
         # Match procedure
         # signaldat = lengtheq(waveformdat[0], waveformdat[1], delta_t)
-        waveform1, waveform2, _ = lengtheq(waveformdat[0], waveformdat[1], delta_t)
+        waveform1, waveform2, _ = lengtheq(
+            waveformdat[0], waveformdat[1], delta_t
+        )
 
         # waveform1 = signaldat[0]
         # waveform2 = signaldat[1]
 
         # alignedwvs = pycbc.waveform.utils.coalign_waveforms(signaldat,hpa)
         # Compute the match to calculate match and shift.
         # Note: The match function from pycbc returns the match of the
         # normalized templates
-        (match_score, shift) = pycbc.filter.matchedfilter.match(waveform1, waveform2)
+        (match_score, shift) = pycbc.filter.matchedfilter.match(
+            waveform1, waveform2
+        )
 
         # Coalign the waveforms using pycbc coalign.
-        waveform1, waveform2 = pycbc.waveform.utils.coalign_waveforms(waveform1, waveform2)
+        waveform1, waveform2 = pycbc.waveform.utils.coalign_waveforms(
+            waveform1, waveform2
+        )
 
         # Normalize the waveforms
 
         waveform1 = waveform1 / norm(waveform1)
         waveform2 = waveform2 / norm(waveform2)
 
         try:
-            (match_score, shift) = pycbc.filter.matchedfilter.match(waveform1, waveform2)
+            (match_score, shift) = pycbc.filter.matchedfilter.match(
+                waveform1, waveform2
+            )
         except BaseException:
             message("Final match couldn't be found!")
             match_score = None
             shift = None
 
-        match.append({"Waveforms": [waveform1, waveform2], "Match score": match_score, "Shift": shift})
+        match.append(
+            {
+                "Waveforms": [waveform1, waveform2],
+                "Match score": match_score,
+                "Shift": shift,
+            }
+        )
     return match
 
 
 def pmmatch_wfs(waveforms, offset=25, crop=None):
     """
     Match function for post merger waveforms.
 
@@ -2401,22 +2553,22 @@
                 The pairs of waveforms to match
                 in the format
                 [[wf1_pair1, wf2_pair2], [wf1_pair_2, wf2_pair2], ...].
     offset : int
              Number of indices to shift the data.
     crop : string
            A string to decide how to crop the waveforms.
-		   The available Options are 1. `signal` 2. `template` 3. `both`.
+                   The available Options are 1. `signal` 2. `template` 3. `both`.
 
     Returns
     -------
     matchdet : a list of dicts
-			   A list of dictionaries.
+                           A list of dictionaries.
                Each contains
-			       1. the waveform pair,
+                               1. the waveform pair,
                    2. the match score,
                    3. the shift index. to maximize the match.
 
     """
     matchdet = []
     for waveformdat in waveforms:
         signal, template = waveformdat
@@ -2457,23 +2609,33 @@
             delta_t = template.delta_t
         except BaseException:
             delta_t = 1
             template = pycbc.types.timeseries.TimeSeries(template, delta_t)
 
         # message(type(signal), type(template))
         # Align the waveforms in phase
-        signal_al, template_al = pycbc.waveform.utils.coalign_waveforms(signal, template)
+        signal_al, template_al = pycbc.waveform.utils.coalign_waveforms(
+            signal, template
+        )
 
         # message(np.where(np.array(signalp_al)!=0))
 
         # Compute the match score
-        (matchscore, finalshift) = pycbc.filter.matchedfilter.match(signal_al, template_al)
+        (matchscore, finalshift) = pycbc.filter.matchedfilter.match(
+            signal_al, template_al
+        )
 
         # message('+ The match score, shift are %f, %d'%(matchscore, finalshift))
-        matchdet.append({"Waveforms": [signal_al, template_al], "Match score": matchscore, "Shift": finalshift})
+        matchdet.append(
+            {
+                "Waveforms": [signal_al, template_al],
+                "Match score": matchscore,
+                "Shift": finalshift,
+            }
+        )
 
     return matchdet
 
 
 def roll(tsdata, i_roll, is_ts=False):
     """Roll the data circularly. Circular counterpart of shiftmatched function.
 
@@ -2483,15 +2645,15 @@
             1D data vector in the form of a list/ numpy array or timeseries.
     i_roll : int
              The number of indices to roll the array.
 
     Returns
     -------
     rolled_waveform : 1d array or(pycbc TimeSeries object
-					  The rolled wavefrom.
+                                          The rolled wavefrom.
     """
 
     flag = 0
     if is_ts:
         try:
             # Assign the time step.
             delta_t = tsdata.delta_t
@@ -2503,39 +2665,44 @@
     tsdata = np.array(tsdata)
     # Break the array into two parts as last i + first i entries.
     arr1 = tsdata[-i_roll:]
     arr2 = tsdata[:-i_roll]
     # Join the two arrays and return them
     if flag == 1:
         rolled_waveform = pycbc.types.timeseries.TimeSeries(
-            np.transpose(np.concatenate((np.transpose(arr1), np.transpose(arr2)))), delta_t
+            np.transpose(
+                np.concatenate((np.transpose(arr1), np.transpose(arr2)))
+            ),
+            delta_t,
         )
 
     else:
-        rolled_waveform = np.transpose(np.concatenate((np.transpose(arr1), np.transpose(arr2))))
+        rolled_waveform = np.transpose(
+            np.concatenate((np.transpose(arr1), np.transpose(arr2)))
+        )
 
     return rolled_waveform
 
 
 def smoothen(func_x, win, order, xdata=None, to_plot=False):
     """Use the Savitzky-Golay Filter to smoothen the data.
-	Show the plots if plot=`yes`.
+        Show the plots if plot=`yes`.
 
-	Parameters
+        Parameters
     ----------
     func_x : 1d array
-			 The y axis.
-	win :  int
-		  Window for smoothening. Must be odd.
+                         The y axis.
+        win :  int
+                  Window for smoothening. Must be odd.
     order : int
             The order of the polynomial used for interpolation.
-	x : 1d array, optional.
-		The 1D list or numpy array, to plot the smoothened function.
-		Only required if to_plot=True.
-	to_plot : bool
+        x : 1d array, optional.
+                The 1D list or numpy array, to plot the smoothened function.
+                Only required if to_plot=True.
+        to_plot : bool
               True or False. Whether or not to display the plot.
 
     Returns
     -------
     ydata : 1d array
             The Savgol filtered list.
 
@@ -2559,47 +2726,55 @@
     """Function to bin the data and interpolate it at specified width and order.
 
     Parameters
     ----------
     xdata :  1d array
              1D list or numpy array.
     func_x : 1d array
-			 The y axis.
+                         The y axis.
     width : int
-			Window size for smoothening,
+                        Window size for smoothening,
     order : int
-			Order of the polynomial used for interpolation.
+                        Order of the polynomial used for interpolation.
     to_plot : bool
-			  True or False. To plot or not plot the results.
+                          True or False. To plot or not plot the results.
 
     Returns
     -------
     hist : list
            [binloc, yvals], The location of the bins and
-		   the y values associated with the bins.
+                   the y values associated with the bins.
 
     """
 
     # Interpolation orders
     kind = [0, "linear", "quadratic", "cubic"]
     # Parse width
     width = int(width)
     # Number of bins
     nbins = int(len(xdata) / width)
     # Location of the bins
-    binloc = [np.mean(xdata[width * index : width * index + width]) for index in range(0, nbins + 1)]
+    binloc = [
+        np.mean(xdata[width * index : width * index + width])
+        for index in range(0, nbins + 1)
+    ]
     # message(binloc)
     # Assigning y values to the bins
-    yvals = [np.mean(func_x[width * index : width * index + width]) for index in range(0, nbins + 1)]
+    yvals = [
+        np.mean(func_x[width * index : width * index + width])
+        for index in range(0, nbins + 1)
+    ]
     # Assigning x values to the smoothened data
     # xf=x[width:-(width)/2]
     y_final = yvals
     # Interpolate if specified order is more than 0
     if order != 0:
-        y_interp_func = scipy.interpolate.interp1d(binloc, yvals, kind=kind[order])
+        y_interp_func = scipy.interpolate.interp1d(
+            binloc, yvals, kind=kind[order]
+        )
     # Reassign yf
     y_final = y_interp_func(binloc)
     # Set xf to binloc if order=0
     # if order==0:
     #       xf=binloc
     # y = signal.savgol_filter(func_x,win,order)
     if to_plot:
@@ -2619,20 +2794,20 @@
     """Function to smoothen data. Moving average over the window width.
 
     Parameters
     ----------
     func_x : 1d array
              A list or numpy array of y axis.
     Width : int
-			The width of the moving average window.
+                        The width of the moving average window.
 
     Returns
     -------
     func_x_avgd : 1d array
-				  1D array of moving averaged y axis.
+                                  1D array of moving averaged y axis.
 
     """
 
     # message(len(func_x))
     # List to store smoothened data
     func_x_avgd = []
     # Calculate the moving-average upto last but width num of points
@@ -2651,43 +2826,46 @@
 def interpolate_wfs(ts_data, interp_func, delta_t=None, **kwargs):
     """Function to interpolate a list of timeseries data using
     the user specified interp_func function and the keyword arguments.
 
     Parameters
     ----------
     ts_data : list
-			  The 1d data. A list of waveforms
-			  as a list or numpy array or
-		      pycbc TimeSeries.
+                          The 1d data. A list of waveforms
+                          as a list or numpy array or
+                      pycbc TimeSeries.
     interp_fun : function
                 An interpolating function.
     delta_t : float
-			  Timestep.
+                          Timestep.
     ``**kwargs`` : keyword arguments
-				   additional arguments to the user specified interp_func.
+                                   additional arguments to the user specified interp_func.
 
     Returns
     -------
     interp_data : list
-				  A list containing interpolated data.
+                                  A list containing interpolated data.
 
     """
 
     # List for storing the interpolated data function
     interp_data = []
     # Loop over items in input
     for wfs in ts_data:
         if not delta_t:
             try:
                 # Find sampling time_step
                 delta_t = wfs.delta_t
                 timeaxis = wfs.sample_times
 
             except BaseException:
-                message("Input is not a TimeSeries. Please supply gridspacing as delta_t", message_verbosity=0)
+                message(
+                    "Input is not a TimeSeries. Please supply gridspacing as delta_t",
+                    message_verbosity=0,
+                )
         else:
             timeaxis = np.arange(0, len(wfs) * delta_t, delta_t)
 
         # Interpolate using the supplied function. The keyword arguments
         # supplied to the fuction are the keyword arguments to be supplied
         # to the interpolating function)
         # Append to the list of interpolated data function
@@ -2699,78 +2877,92 @@
 def resample(interp_data, new_delta_t, epoch, length, old_delta_t=None):
     """Function to generate timeseries out of the given interpolated data
     function, epoch,sampling frequency, length(duration).
 
     Parameters
     ----------
     interp_data : 1d array
-				  The yaxis to be interpolated.
+                                  The yaxis to be interpolated.
     epoch : float
-			The starting point in time.
+                        The starting point in time.
     delta_t : float
-			  New grid spacing to be sampled at.
+                          New grid spacing to be sampled at.
     length : int
              The duration of x axis.
 
     Returns
     -------
 
     data : list
-		   A list containing resampled data as pycbc TimeSeries.
+                   A list containing resampled data as pycbc TimeSeries.
     """
 
     data = []
     # Loop over objects in interp_data
     for i in range(len(interp_data)):
         if not old_delta_t:
             try:
                 old_delta_t = interp_data[i].delta_t
 
             except BaseException:
-                message("Input is not a TimeSeries. Please supply gridspacing as delta_t", message_verbosity=0)
+                message(
+                    "Input is not a TimeSeries. Please supply gridspacing as delta_t",
+                    message_verbosity=0,
+                )
         else:
-            interp_data[i] = pycbc.types.timeseries.TimeSeries(interp_data[i], old_delta_t)
+            interp_data[i] = pycbc.types.timeseries.TimeSeries(
+                interp_data[i], old_delta_t
+            )
 
         # Prepare timeaxis
-        timeaxis = np.linspace(epoch, epoch + length, int(length / new_delta_t))
+        timeaxis = np.linspace(
+            epoch, epoch + length, int(length / new_delta_t)
+        )
         # Append the timeseries to the data list
         ydata = interp_data[i](timeaxis)
-        data.append(pycbc.types.timeseries.TimeSeries(ydata, new_delta_t, epoch=epoch))
+        data.append(
+            pycbc.types.timeseries.TimeSeries(ydata, new_delta_t, epoch=epoch)
+        )
     # Return the list of samples timeseries
     return data
 
 
 def interp_resam_wfs(wavf_data, old_taxis, new_taxis, kind="cubic", k=None):
     """Wrapper function for interpolation and resampling.
 
     Parameters
     ----------
     wavf_data : 1d array
                 The yaxis to be interpolated,
     old_taxis, new_taxis : 1darray
-						   Old and New time axis.
+                                                   Old and New time axis.
 
     Returns
     -------
     resam_wf_data : 1d array
                     Interpolated and resampled data.
     """
     # from scipy.interpolate import interp1d
 
     amp, phase = xtract_camp_phase(wavf_data.real, wavf_data.imag)
 
     # Interpolate
     if k is not None:
-        from scipy.interpolate import InterpolatedUnivariateSpline as interpolator
+        from scipy.interpolate import (
+            InterpolatedUnivariateSpline as interpolator,
+        )
 
         interp_amp_data = interpolator(old_taxis, amp, k=k)
         amp_res = interp_amp_data.get_residual()
         interp_phase_data = interpolator(old_taxis, phase, k=k)
         phase_res = interp_phase_data.get_residual()
-        message(f"Amplitude residue {amp_res} \t Phase residue {phase_res}", message_verbosity=2)
+        message(
+            f"Amplitude residue {amp_res} \t Phase residue {phase_res}",
+            message_verbosity=2,
+        )
     else:
         from scipy.interpolate import interp1d as interpolator
 
         interp_amp_data = interpolator(old_taxis, amp, kind=kind)
         interp_phase_data = interpolator(old_taxis, phase, kind=kind)
 
     # Resample
@@ -2798,15 +2990,17 @@
     1 : int
         The progress bar is messageed to stdout.
     """
 
     if normalize == "yes":
         final_progress = 98
         normalized_total_counts = final_progress * 10
-        present_count = int(normalized_total_counts * present_count / total_counts)
+        present_count = int(
+            normalized_total_counts * present_count / total_counts
+        )
         total_counts = normalized_total_counts
 
     # present_count = comm.gather(count,root=rank)
     else:
         final_progress = int(total_counts / 10)
 
     present_stage = int(present_count / 10)
```

### Comparing `waveformtools-2023.6.5/waveformtools.egg-info/PKG-INFO` & `waveformtools-2023.7.14/waveformtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveformtools
-Version: 2023.6.5
+Version: 2023.7.14
 Summary:  Tools for working with numerical relativity and waveforms data 
 Home-page: https://gitlab.com/vaishakp/waveformtools
 Author: Vaishak Prasad
 Author-email: Vaishak Prasad <vaishakprasad@gmail.com>
 Project-URL: Homepage, https://gitlab.com/vaishakp/waveformtools
 Project-URL: Bug Tracker, https://gitlab.com/vaishakp/waveformtools/issues
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 License-File: LICENSE
 
 [[Project landing page]](https://sites.google.com/view/waveformtools/home)
 [![pipeline status](https://gitlab.com/vaishakp/waveformtools/badges/main/pipeline.svg)](https://gitlab.com/vaishakp/waveformtools/commits/main)
 [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://gitlab.com/vaishakp/waveformtools/commits/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/waveformtools/badge/?version=latest)](https://waveformtools.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![PyPI version](https://badge.fury.io/py/waveformtools.svg)](https://badge.fury.io/py/waveformtools)
+[![PyPI version](docs/vers_badge.svg)](https://pypi.org/project/waveformtools/)
 # Waveformtools 
 
 
 This is a python module for the handling and analysis of waveforms and data from Numerical Relativity codes, and for carrying out gravitational wave data analysis.  
 
 waveformtools is a numerical relativity data handling package that was written to aid the handling and analysis of numerical relativity data.
```

### Comparing `waveformtools-2023.6.5/waveformtools.egg-info/SOURCES.txt` & `waveformtools-2023.7.14/waveformtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

