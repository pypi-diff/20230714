# Comparing `tmp/animate-transit-0.1.tar.gz` & `tmp/animate-transit-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/animate-transit-0.1.tar", last modified: Thu Jul 13 20:31:30 2023, max compression
+gzip compressed data, was "dist/animate-transit-1.0.tar", last modified: Thu Jul 13 22:24:58 2023, max compression
```

## Comparing `animate-transit-0.1.tar` & `animate-transit-1.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 seanobrien   (502) staff       (20)        0 2023-07-13 20:31:30.000000 animate-transit-0.1/
--rw-r--r--   0 seanobrien   (502) staff       (20)       57 2023-07-13 20:31:30.000000 animate-transit-0.1/PKG-INFO
--rw-r--r--   0 seanobrien   (502) staff       (20)      111 2023-07-12 15:30:30.000000 animate-transit-0.1/README.md
-drwxr-xr-x   0 seanobrien   (502) staff       (20)        0 2023-07-13 20:31:30.000000 animate-transit-0.1/animate_transit/
--rw-r--r--   0 seanobrien   (502) staff       (20)       19 2023-07-12 14:59:21.000000 animate-transit-0.1/animate_transit/__init__.py
--rw-r--r--   0 seanobrien   (502) staff       (20)     9244 2023-07-13 20:27:38.000000 animate-transit-0.1/animate_transit/main.py
-drwxr-xr-x   0 seanobrien   (502) staff       (20)        0 2023-07-13 20:31:30.000000 animate-transit-0.1/animate_transit.egg-info/
--rw-r--r--   0 seanobrien   (502) staff       (20)       57 2023-07-13 20:31:30.000000 animate-transit-0.1/animate_transit.egg-info/PKG-INFO
--rw-r--r--   0 seanobrien   (502) staff       (20)      264 2023-07-13 20:31:30.000000 animate-transit-0.1/animate_transit.egg-info/SOURCES.txt
--rw-r--r--   0 seanobrien   (502) staff       (20)        1 2023-07-13 20:31:30.000000 animate-transit-0.1/animate_transit.egg-info/dependency_links.txt
--rw-r--r--   0 seanobrien   (502) staff       (20)       30 2023-07-13 20:31:30.000000 animate-transit-0.1/animate_transit.egg-info/requires.txt
--rw-r--r--   0 seanobrien   (502) staff       (20)       16 2023-07-13 20:31:30.000000 animate-transit-0.1/animate_transit.egg-info/top_level.txt
--rw-r--r--   0 seanobrien   (502) staff       (20)       38 2023-07-13 20:31:30.000000 animate-transit-0.1/setup.cfg
--rw-r--r--   0 seanobrien   (502) staff       (20)      626 2023-07-12 15:14:53.000000 animate-transit-0.1/setup.py
+drwxr-xr-x   0 seanobrien   (502) staff       (20)        0 2023-07-13 22:24:58.000000 animate-transit-1.0/
+-rw-r--r--   0 seanobrien   (502) staff       (20)      135 2023-07-13 22:24:58.000000 animate-transit-1.0/PKG-INFO
+-rw-r--r--   0 seanobrien   (502) staff       (20)      111 2023-07-13 22:15:03.000000 animate-transit-1.0/README.md
+drwxr-xr-x   0 seanobrien   (502) staff       (20)        0 2023-07-13 22:24:58.000000 animate-transit-1.0/animate_transit/
+-rw-r--r--   0 seanobrien   (502) staff       (20)       19 2023-07-13 22:17:23.000000 animate-transit-1.0/animate_transit/__init__.py
+-rw-r--r--   0 seanobrien   (502) staff       (20)     9532 2023-07-13 22:15:03.000000 animate-transit-1.0/animate_transit/main.py
+drwxr-xr-x   0 seanobrien   (502) staff       (20)        0 2023-07-13 22:24:58.000000 animate-transit-1.0/animate_transit.egg-info/
+-rw-r--r--   0 seanobrien   (502) staff       (20)      135 2023-07-13 22:24:58.000000 animate-transit-1.0/animate_transit.egg-info/PKG-INFO
+-rw-r--r--   0 seanobrien   (502) staff       (20)      311 2023-07-13 22:24:58.000000 animate-transit-1.0/animate_transit.egg-info/SOURCES.txt
+-rw-r--r--   0 seanobrien   (502) staff       (20)        1 2023-07-13 22:24:58.000000 animate-transit-1.0/animate_transit.egg-info/dependency_links.txt
+-rw-r--r--   0 seanobrien   (502) staff       (20)       30 2023-07-13 22:24:58.000000 animate-transit-1.0/animate_transit.egg-info/requires.txt
+-rw-r--r--   0 seanobrien   (502) staff       (20)       16 2023-07-13 22:24:58.000000 animate-transit-1.0/animate_transit.egg-info/top_level.txt
+-rw-r--r--   0 seanobrien   (502) staff       (20)       38 2023-07-13 22:24:58.000000 animate-transit-1.0/setup.cfg
+-rw-r--r--   0 seanobrien   (502) staff       (20)      715 2023-07-13 22:15:03.000000 animate-transit-1.0/setup.py
+drwxr-xr-x   0 seanobrien   (502) staff       (20)        0 2023-07-13 22:24:58.000000 animate-transit-1.0/tests/
+-rw-r--r--   0 seanobrien   (502) staff       (20)      149 2023-07-13 22:15:03.000000 animate-transit-1.0/tests/test_phase.py
+-rw-r--r--   0 seanobrien   (502) staff       (20)      966 2023-07-13 22:15:03.000000 animate-transit-1.0/tests/test_transitdepth.py
```

### Comparing `animate-transit-0.1/animate_transit/main.py` & `animate-transit-1.0/animate_transit/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,17 @@
         u2_2 (float, optional): Quadratic limb darkening coefficient for object 2 (default: None)
     """
     def __init__(self, n_pixs, R1, R2, a_R1, b, theta, L2_L1, u1_1=None, u2_1=None, u1_2=None, u2_2=None):
         self.n_pixs = n_pixs    # number of pixels in grid (npixs by npixs)
 
         pix_per_unit = n_pixs/(3*R1+2*(a_R1*R1)+3*R2)  #conversion factor between pixels and unit
 
+        if R1<=0 or R2<=0:
+            raise ValueError("Radii cannot be negative")
+
         self.R1 = pix_per_unit*R1  # radius of object 1 (stationary object) in same units as R2
         self.R2 = pix_per_unit*R2  # radius of object 2 in same units as R1
 
         self.a_R1 = a_R1        # orbital distance over radius of object 1
         self.b = b              # impact parameter
         self.theta = theta      # spin-orbit angle
         self.grid1 = np.zeros((self.n_pixs, self.n_pixs))   # grid for object 1 (serves as background grid)
@@ -67,15 +70,15 @@
         return self.grid1
 
     def model_object2(self, phase):
         """
         Models the flux of the orbiting object at the given phase
 
         Args:
-            phase (float): Orbital phase of object 2 to model
+            phase (float): Orbital phase of object 2 to model where transit occurs at phase=0.
             
         Returns:
             grid (np.ndarray of float): 2D pixel map showing visualisation of the system
         """
         grid = self.grid1.copy()
 
         ## calculate pixel coordinates of centre of object 2 (x1 and y1) from phase (using orbital properties)
@@ -105,19 +108,21 @@
     Args:
         file_list (:obj:`list` of :obj:`str`): List of filepaths to individual images to be compiled into gif
         output_file (str): Filename for output gif
 
     Returns:
         None
     """
-    with imageio.get_writer('{}.gif'.format(output_file), mode='I', duration=0.1) as writer:
+    with imageio.get_writer('{}'.format(output_file), mode='I', duration=0.1) as writer:
         for file in file_list:
             image = imageio.imread(file)
             writer.append_data(image)
 
+    print("Gif written to {}".format(output_file))
+
 def normalised_flux(grid, grid1):
     """
     Calculates the normalised flux for the given model by comparing to the background pixel image of just the stationary object
 
     Args:
         grid (np.ndarray of float): Output model grid from model_object2 for given phase
         grid1 (np.ndarray of float): 2D pixel map of object 1 (returned from model_object1)
@@ -193,16 +198,16 @@
         flux_tmp = flux_arr[phase_arr<=phase]
 
         fig, (ax1, ax2) = plt.subplots(2, figsize=(8,15))
         
         # Plots visualisation of the system
         ax1.imshow(model)
         ax1.axis("off")
-
         # Plots light curve
+        #TODO fix number of decimal places for normalised flux so the subplots don't jump around (jump jump, jump around!)
         ax2.scatter(phase_tmp, flux_tmp, marker='.', c='c')
         ax2.set_xlim(min(phase_arr), max(phase_arr))
 
         ax2.set_xlabel("Phase")
         ax2.set_ylabel("Normalized Flux")
 
         #Sets the aspect ratios of the subplots to be the same
```

### Comparing `animate-transit-0.1/setup.py` & `animate-transit-1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,9 +19,11 @@
 
     name="animate-transit",
 
     version=get_property("__version__", "animate_transit"),
 
     packages=find_packages(),
 
+    description="Generates an animation and lightcurve for a transiting 2-body system",
+
     install_requires=get_requires()
 )
```

