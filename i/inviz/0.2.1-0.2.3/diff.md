# Comparing `tmp/inviz-0.2.1.tar.gz` & `tmp/inviz-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inviz-0.2.1.tar", last modified: Wed Jul 12 08:20:13 2023, max compression
+gzip compressed data, was "inviz-0.2.3.tar", last modified: Thu Jul 13 22:24:17 2023, max compression
```

## Comparing `inviz-0.2.1.tar` & `inviz-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-12 08:20:13.456552 inviz-0.2.1/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.2.1/LICENSE
--rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.2.1/MANIFEST.in
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-07-12 08:20:13.456552 inviz-0.2.1/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1641 2023-07-12 08:18:52.000000 inviz-0.2.1/README.md
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-12 08:20:13.456552 inviz-0.2.1/inviz/
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-12 08:20:13.456552 inviz-0.2.1/inviz/inviz.egg-info/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-07-12 08:20:13.000000 inviz-0.2.1/inviz/inviz.egg-info/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-07-12 08:20:13.000000 inviz-0.2.1/inviz/inviz.egg-info/SOURCES.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-07-12 08:20:13.000000 inviz-0.2.1/inviz/inviz.egg-info/dependency_links.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)       89 2023-07-12 08:20:13.000000 inviz-0.2.1/inviz/inviz.egg-info/requires.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-07-12 08:20:13.000000 inviz-0.2.1/inviz/inviz.egg-info/top_level.txt
--rwxr-xr-x   0 jswen     (1000) jswen     (1000)    10524 2023-07-12 08:18:52.000000 inviz-0.2.1/inviz/inviz.py
--rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-07-12 08:20:13.456552 inviz-0.2.1/setup.cfg
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1100 2023-07-12 08:18:52.000000 inviz-0.2.1/setup.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-13 22:24:17.169098 inviz-0.2.3/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.2.3/LICENSE
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.2.3/MANIFEST.in
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-07-13 22:24:17.169098 inviz-0.2.3/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1642 2023-07-13 22:19:19.000000 inviz-0.2.3/README.md
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-13 22:24:17.159098 inviz-0.2.3/inviz/
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-13 22:24:17.169098 inviz-0.2.3/inviz/inviz.egg-info/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-07-13 22:24:17.000000 inviz-0.2.3/inviz/inviz.egg-info/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-07-13 22:24:17.000000 inviz-0.2.3/inviz/inviz.egg-info/SOURCES.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-07-13 22:24:17.000000 inviz-0.2.3/inviz/inviz.egg-info/dependency_links.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      103 2023-07-13 22:24:17.000000 inviz-0.2.3/inviz/inviz.egg-info/requires.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-07-13 22:24:17.000000 inviz-0.2.3/inviz/inviz.egg-info/top_level.txt
+-rwxr-xr-x   0 jswen     (1000) jswen     (1000)    10766 2023-07-13 22:19:19.000000 inviz-0.2.3/inviz/inviz.py
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-07-13 22:24:17.169098 inviz-0.2.3/setup.cfg
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1139 2023-07-13 22:23:34.000000 inviz-0.2.3/setup.py
```

### Comparing `inviz-0.2.1/LICENSE` & `inviz-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `inviz-0.2.1/PKG-INFO` & `inviz-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.2.1
+Version: 0.2.3
 Summary: An interactive visualizer to help explore high-dimensional data and its observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inviz-0.2.1/README.md` & `inviz-0.2.3/README.md`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 If no errors appear, all the dependencies were installed correctly and we're ready to start visualizing!
 
 ### Example
 Download and run the `live_data_example` notebook in the [tutorials](tutorials) folder to see an example of how inviz can be used.
 
 Here's an example of InViz in an astrophysics context! The parameters come from a specific dark matter model, and the observables are the matter power spectrum and CMB anisotropy power spectra.
 
-![example output](images/example2.png)
+![example output](images/example2.png)
```

### Comparing `inviz-0.2.1/inviz/inviz.egg-info/PKG-INFO` & `inviz-0.2.3/inviz/inviz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.2.1
+Version: 0.2.3
 Summary: An interactive visualizer to help explore high-dimensional data and its observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inviz-0.2.1/inviz/inviz.py` & `inviz-0.2.3/inviz/inviz.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,78 +31,75 @@
     myfunc: callable
         a user-provided function that returns parameters. can return more than one
         set of parameters if the "grouped" option is True
 
     myfunc_args: tuple
         arguments for user-provided function
 
-    grouped: boolean
-        specifies if user-provided function returns more than one set of parameters
-
     plot_type: string
         specifies how the data should be visualized. currently can pick either 'Curve'
         or 'Scatter'
 
     plot_opts: holoviews Options object
         customization options for the observable plot. see Holoviews documentation
     """
     
     def __init__(
         self, 
         name: str | list[str] = None, 
         parameters: dict | list[dict] = None, 
         myfunc: Callable = None,
         myfunc_args: tuple = None, 
-        grouped: bool = False, 
         plot_type: str | list[str] = None,
         plot_opts: type[opts] | list[type[opts]] = None,
         latex_labels: dict = None
     ):
-        self.name = [name]
-        self.parameters = parameters
-        if parameters is not None:
+        if isinstance(name, str):
+            self.name = [name]
+        else:
+            self.name = name
+        if isinstance(parameters, dict):
             self.parameters = [parameters]
+        else:
+            self.parameters = parameters
         self.myfunc = myfunc
         self.myfunc_args = myfunc_args
-        self.plot_type = plot_type
-        if plot_type is not None:
+        if isinstance(plot_type, str):
             self.plot_type = [plot_type]
-        self.plot_opts = plot_opts
-        if plot_opts is not None:
-            self.plot_opts = [plot_opts]
-        self.grouped = grouped
-        self.latex_labels = latex_labels
-        if self.grouped:
-            self.name = name
-            self.parameters = parameters
+        else:
             self.plot_type = plot_type
+        if isinstance(plot_opts, hv.core.options.Options):
+            self.plot_opts = [plot_opts]
+        else:
             self.plot_opts = plot_opts
+        self.latex_labels = latex_labels
         self.number = len(self.name)
     
     def properties(self):
-        if self.grouped:
-            print("InViz Grouped Observable")
+        if len(self.name) > 1:
+            print("InViz Grouped Observables")
             for i in range(len(self.name)):
                 print(f"\t- Observable {i+1}: {self.name[i]}")
         else:
             print("InViz Observable")
-            print(f"Name: {self.name}")
+            print(f"Name: {self.name[0]}")
         
     def generate_plot(self, index: int):
         self.plots_list = []
         if self.myfunc and self.myfunc_args is not None:
             computed_data = self.myfunc(index, *self.myfunc_args)
             self.number = len(computed_data)
         for i in range(0, self.number):
             hv_element = getattr(hv, self.plot_type[i])
             if self.parameters is not None:
                 dataset = self.parameters[i]
                 kdim = list(dataset.keys())[0]
                 vdim = list(dataset.keys())[1]
-                plot = hv_element(dataset[index], kdim, vdim, label=self.name[i])
+                indexed_data = (dataset[kdim][index], dataset[vdim][index])
+                plot = hv_element(indexed_data, kdim, vdim, label=self.name[i])
             elif computed_data:
                 dataset = computed_data[i]
                 kdim = list(dataset.keys())[0]
                 vdim = list(dataset.keys())[1]
                 plot = hv_element(dataset, kdim, vdim, label=self.name[i])
             # set defaults
             plot.opts(
@@ -122,14 +119,17 @@
     def draw_plot(self, index):
         layout = hv.Layout(self.generate_plot(index))
         return layout.opts(shared_axes=False)
         
 
 #  given a param name, find corresponding latex-formatted param name
 def lookup_latex_label(param, latex_dict):
+    # handle default case of no latex paramname dictionary
+    if latex_dict is None:
+        latex_dict = dict()
     try:
         latex_param = latex_dict[param]
         label = r'$${}$$'.format(latex_param)
         return label
     except KeyError:
         label = param
         return label
@@ -137,29 +137,43 @@
 
 def viz(
     data, 
     observables: list = None, 
     show_observables: bool = True, 
     latex_dict: dict = None
 ):
-    # handle default case of no latex paramname dictionary
-    if latex_dict is None:
-        latex_dict = dict()
     # setting Panel widgets for user interaction
     variables = data.columns.values.tolist()
-    var1 = pn.widgets.Select(value=variables[1], name='Horizontal Axis', options=variables)
-    var2 = pn.widgets.Select(value=variables[2], name='Vertical Axis', options=variables)
-    cmap_var = pn.widgets.Select(value=variables[0], name='Colormapped Parameter', options=variables)
-    cmap_option = pn.widgets.Checkbox(value=True, name='Show Colormap', align='end')
+    var1 = pn.widgets.Select(
+        value=variables[1], 
+        name='Horizontal Axis', 
+        options=variables
+    )
+    var2 = pn.widgets.Select(
+        value=variables[2], 
+        name='Vertical Axis', 
+        options=variables
+    )
+    cmap_var = pn.widgets.Select(
+        value=variables[0], 
+        name='Colormapped Parameter', 
+        options=variables
+    )
+    cmap_option = pn.widgets.Checkbox(
+        value=True, 
+        name='Show Colormap', 
+        align='end'
+    )
 
     # function for generating the scatter plot, given 2 dimensions as x and y axes, and an additional dimension to colormap
     # to the points on the plot. Also has an option to show or hide the colormap
     def plot_data(kdim1, kdim2, colordim, showcmap):
         if showcmap == True:
-            cmapping = opts.Points(color=dim(colordim),
+            cmapping = opts.Points(
+                color=dim(colordim),
                 colorbar=True,
                 cmap='GnBu_r')
         else:
             cmapping = opts.Points(color='grey', colorbar=True)
         hover = HoverTool(tooltips=None)
         xlabel = lookup_latex_label(kdim1, latex_dict)
         ylabel = lookup_latex_label(kdim2, latex_dict)
@@ -188,21 +202,33 @@
     def hook(plot, element):
         plot.handles['table'].autosize_mode = "none"
         for column in plot.handles['table'].columns:
             column.width = 100
     
     # function to generate a table of all the selected points
     def make_table(kdim1, kdim2, colordim):
-        table_options = opts.Table(height=300, width=1000, hooks=[hook], bgcolor='#f5f5f5')
-        table = hv.DynamicMap(lambda index: hv.Table(data.iloc[index], kdims=[kdim1, kdim2, colordim]), streams=[selection])
+        table_options = opts.Table(
+            height=300, 
+            width=1000, 
+            hooks=[hook], 
+            bgcolor='#f5f5f5'
+        )
+        table = hv.DynamicMap(
+            lambda index: hv.Table(data.iloc[index], kdims=[kdim1, kdim2, colordim]), 
+            streams=[selection]
+        )
         return table.opts(table_options).relabel('Selected Points')
     
     
     # generate the table
-    selected_table = pn.bind(make_table, kdim1=var1, kdim2=var2, colordim=cmap_var)
+    selected_table = pn.bind(
+        make_table, 
+        kdim1=var1, 
+        kdim2=var2, 
+        colordim=cmap_var)
     
     #table_stream = streams.Selection1D(source=selected_table)
     
     # handles the null selection case and multiple selections
     plots = {}
     # get total number of plots to draw from list of observables
     plotting_info = {}
@@ -246,15 +272,18 @@
         for list_of_plots in plots_list:
             overlay = hv.Overlay(list_of_plots).opts(show_legend=False)
             layout = layout + overlay
         layout.opts(shared_axes=False).cols(3)
         return layout
     
     # put it all together using Panel
-    dashboard = pn.Column(pn.Row(var1, var2, cmap_var, cmap_option), pn.Row(points_dmap, selected_table))
+    dashboard = pn.Column(
+        pn.Row(var1, var2, cmap_var, cmap_option), 
+        pn.Row(points_dmap, selected_table)
+    )
     
     if show_observables == True:
         observables_dmap = hv.DynamicMap(plot_observables, streams=[selection]).opts(framewise=True)
         observables_pane = pn.panel(observables_dmap)
         dashboard = pn.Column(dashboard, observables_pane)
     
     return dashboard
```

### Comparing `inviz-0.2.1/setup.py` & `inviz-0.2.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "inviz",
-    version = "0.2.1",
+    version = "0.2.3",
     author = "James Wen",
     author_email = "jswen@usc.edu",
     description = ("An interactive visualizer to help explore high-dimensional data and its observables."),
     license = "MIT",
     keywords = "interactive visualizer cosmology",
     url = "http://packages.python.org/inviz",
     py_modules=["inviz"],
@@ -24,11 +24,12 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
     ],
     python_requires='>=3.8',
     install_requires=["holoviews==1.15.4",
                       "panel==0.14.4",
                       "spatialpandas==0.4.7",
+                      "param==1.13.0",
                       "numpy>=1.20, <1.24",
                       "matplotlib==3.7.1"]
     )
```

