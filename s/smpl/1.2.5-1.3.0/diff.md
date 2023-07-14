# Comparing `tmp/smpl-1.2.5.tar.gz` & `tmp/smpl-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpl-1.2.5.tar", max compression
+gzip compressed data, was "smpl-1.3.0.tar", max compression
```

## Comparing `smpl-1.2.5.tar` & `smpl-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35149 2023-07-14 12:11:05.049019 smpl-1.2.5/LICENSE
--rw-r--r--   0        0        0     3186 2023-07-14 12:11:05.049019 smpl-1.2.5/README.md
--rw-r--r--   0        0        0     2040 2023-07-14 12:11:08.141027 smpl-1.2.5/pyproject.toml
--rw-r--r--   0        0        0      134 2023-07-14 12:11:05.069019 smpl-1.2.5/smpl/__init__.py
--rw-r--r--   0        0        0     3875 2023-07-14 12:11:05.069019 smpl-1.2.5/smpl/data.py
--rw-r--r--   0        0        0       74 2023-07-14 12:11:05.069019 smpl-1.2.5/smpl/debug.py
--rw-r--r--   0        0        0     2088 2023-07-14 12:11:05.069019 smpl-1.2.5/smpl/doc.py
--rw-r--r--   0        0        0    10570 2023-07-14 12:11:05.069019 smpl-1.2.5/smpl/fit.py
--rw-r--r--   0        0        0     2177 2023-07-14 12:11:05.069019 smpl-1.2.5/smpl/functions.py
--rw-r--r--   0        0        0     5185 2023-07-14 12:11:05.069019 smpl-1.2.5/smpl/interpolate.py
--rw-r--r--   0        0        0       62 2023-07-14 12:11:05.069019 smpl-1.2.5/smpl/io.py
--rw-r--r--   0        0        0     3062 2023-07-14 12:11:05.069019 smpl-1.2.5/smpl/latex.py
--rw-r--r--   0        0        0       85 2023-07-14 12:11:05.069019 smpl-1.2.5/smpl/parallel.py
--rw-r--r--   0        0        0    26417 2023-07-14 12:11:05.069019 smpl-1.2.5/smpl/plot.py
--rw-r--r--   0        0        0     6327 2023-07-14 12:11:05.069019 smpl-1.2.5/smpl/plot2d.py
--rw-r--r--   0        0        0     9652 2023-07-14 12:11:05.069019 smpl-1.2.5/smpl/stat.py
--rw-r--r--   0        0        0       66 2023-07-14 12:11:05.069019 smpl-1.2.5/smpl/util.py
--rw-r--r--   0        0        0     5302 2023-07-14 12:11:05.069019 smpl-1.2.5/smpl/wrap.py
--rw-r--r--   0        0        0     4221 1970-01-01 00:00:00.000000 smpl-1.2.5/setup.py
--rw-r--r--   0        0        0     4283 1970-01-01 00:00:00.000000 smpl-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-14 12:11:08.038011 smpl-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3186 2023-07-14 12:11:08.038011 smpl-1.3.0/README.md
+-rw-r--r--   0        0        0     2040 2023-07-14 12:11:11.082042 smpl-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-07-14 12:11:08.058012 smpl-1.3.0/smpl/__init__.py
+-rw-r--r--   0        0        0     3875 2023-07-14 12:11:08.058012 smpl-1.3.0/smpl/data.py
+-rw-r--r--   0        0        0       74 2023-07-14 12:11:08.058012 smpl-1.3.0/smpl/debug.py
+-rw-r--r--   0        0        0     2088 2023-07-14 12:11:08.058012 smpl-1.3.0/smpl/doc.py
+-rw-r--r--   0        0        0    10570 2023-07-14 12:11:08.058012 smpl-1.3.0/smpl/fit.py
+-rw-r--r--   0        0        0     2177 2023-07-14 12:11:08.058012 smpl-1.3.0/smpl/functions.py
+-rw-r--r--   0        0        0     5185 2023-07-14 12:11:08.058012 smpl-1.3.0/smpl/interpolate.py
+-rw-r--r--   0        0        0       62 2023-07-14 12:11:08.058012 smpl-1.3.0/smpl/io.py
+-rw-r--r--   0        0        0     3062 2023-07-14 12:11:08.058012 smpl-1.3.0/smpl/latex.py
+-rw-r--r--   0        0        0       85 2023-07-14 12:11:08.058012 smpl-1.3.0/smpl/parallel.py
+-rw-r--r--   0        0        0    28308 2023-07-14 12:11:08.058012 smpl-1.3.0/smpl/plot.py
+-rw-r--r--   0        0        0     6327 2023-07-14 12:11:08.062012 smpl-1.3.0/smpl/plot2d.py
+-rw-r--r--   0        0        0     9652 2023-07-14 12:11:08.062012 smpl-1.3.0/smpl/stat.py
+-rw-r--r--   0        0        0       66 2023-07-14 12:11:08.062012 smpl-1.3.0/smpl/util.py
+-rw-r--r--   0        0        0     5302 2023-07-14 12:11:08.062012 smpl-1.3.0/smpl/wrap.py
+-rw-r--r--   0        0        0     4221 1970-01-01 00:00:00.000000 smpl-1.3.0/setup.py
+-rw-r--r--   0        0        0     4283 1970-01-01 00:00:00.000000 smpl-1.3.0/PKG-INFO
```

### Comparing `smpl-1.2.5/LICENSE` & `smpl-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smpl-1.2.5/README.md` & `smpl-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `smpl-1.2.5/pyproject.toml` & `smpl-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smpl"
-version = "1.2.5"
+version = "1.3.0"
 description = "SiMPLe plotting and fitting"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/smpl"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `smpl-1.2.5/smpl/data.py` & `smpl-1.3.0/smpl/data.py`

 * *Files identical despite different names*

### Comparing `smpl-1.2.5/smpl/doc.py` & `smpl-1.3.0/smpl/doc.py`

 * *Files identical despite different names*

### Comparing `smpl-1.2.5/smpl/fit.py` & `smpl-1.3.0/smpl/fit.py`

 * *Files identical despite different names*

### Comparing `smpl-1.2.5/smpl/functions.py` & `smpl-1.3.0/smpl/functions.py`

 * *Files identical despite different names*

### Comparing `smpl-1.2.5/smpl/interpolate.py` & `smpl-1.3.0/smpl/interpolate.py`

 * *Files identical despite different names*

### Comparing `smpl-1.2.5/smpl/latex.py` & `smpl-1.3.0/smpl/latex.py`

 * *Files identical despite different names*

### Comparing `smpl-1.2.5/smpl/plot.py` & `smpl-1.3.0/smpl/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -403,74 +403,96 @@
     """
     if "auto_fit" not in kwargs:
         kwargs["auto_fit"] = True
     kwargs = plot_kwargs(kwargs)
     return fit(function=funcs, *adata, **kwargs)
 
 
-def _function(func, xfit, **kwargs):
-    kargs = {}
-    if util.has("fmt", kwargs):
-        kargs["fmt"] = kwargs["fmt"]
-    if util.has("label", kwargs) and kwargs["label"] != "":
-        kargs["label"] = kwargs["label"]
-    if util.has("function_color", kwargs) and kwargs["function_color"] != "":
-        kargs["color"] = kwargs["function_color"]
-    if util.has("sigmas", kwargs) and kwargs["sigmas"] != "":
-        kargs["sigmas"] = kwargs["sigmas"]
-    if util.has("alpha", kwargs) and kwargs["alpha"] != "":
-        kargs["alpha"] = kwargs["alpha"]
-    __function(func, xfit, **kargs)
+def _function(func, xfit,fmt="-",label=None,function_color=None,sigmas=0.0,alpha=0.4, **kwargs):
+
+    #kargs = {}
+    #if util.has("fmt", kwargs):
+    #    kargs["fmt"] = kwargs["fmt"]
+    #if util.has("label", kwargs) and kwargs["label"] != "":
+    #    kargs["label"] = kwargs["label"]
+    #if util.has("function_color", kwargs) and kwargs["function_color"] != "":
+    #    kargs["color"] = kwargs["function_color"]
+    #if util.has("sigmas", kwargs) and kwargs["sigmas"] != "":
+    #    kargs["sigmas"] = kwargs["sigmas"]
+    #if util.has("alpha", kwargs) and kwargs["alpha"] != "":
+    #    kargs["alpha"] = kwargs["alpha"]
+    #__function(func, xfit,  **kargs)
+
+    if label == "":
+        label = None
+    if function_color == "":
+        function_color = None
+    if sigmas == "":
+        sigmas = 0.0
+    if alpha == "":
+        alpha = 0.4
+    __function(func, xfit, fmt=fmt, label=label,color=function_color,sigmas=sigmas, alpha=alpha, **kwargs)
 
 
-def plt_plt(x, y, fmt, color, label, linestyle):
+def plt_plt(x, y, fmt, color, label, linestyle,**kwargs):
     if linestyle is None and fmt is not None:
-        return plt.plot(x, y, fmt, label=label, color=color)
+        return plt.plot(x, y, fmt, label=label, color=color, **kwargs)
     elif linestyle is not None and fmt is None:
-        return plt.plot(x, y, label=label, color=color, linestyle=linestyle)
+        return plt.plot(x, y, label=label, color=color, linestyle=linestyle,**kwargs)
     elif linestyle is None and fmt is None:
-        return plt.plot(x, y, label=label, color=color)
+        return plt.plot(x, y, label=label, color=color,**kwargs)
 
 
 def __function(
     gfunc,
     xlinspace,
     fmt="-",
     label=None,
     color=None,
     hatch=None,
     sigmas=0.0,
     linestyle=None,
     alpha=0.4,
+    **kwargs
 ):
+    # filter unused bad kwargs here to avoid passing them down
+    # TODO it would be better to not pass them down in the first place
+    for key in ["xaxis","yaxis","xvar","xmin","xmax","xlabel","ylabel","bins","binunc","bbox_to_anchor","tight","residue","lpos","interpolate","params","also_fit","init","frange","epsfcn","units","fselector","maxfev","sortbyx","xerror","yerror","fixed_params","autotqdm","fitter",
+                "title","where","save", "prange","ss","also_data", "auto_fit","data_sigmas", "logy", "logx", "data_color", "fit_color", "fit_fmt", "show", "size", "number_format", "selector", "fitinline", "grid", "hist", "stairs", "capsize", "axes",  "xspace",  "extrapolate", "extrapolate_min", "extrapolate_max", "extrapolate_fmt", "extrapolate_hatch",
+                "function_color", "residue_err", "interpolate_fmt", "interpolate_label", "ncol", "steps","interpolator",
+                "next_color",
+                ]:
+        if key in kwargs:
+            del kwargs[key]
     func = gfunc
     x = xlinspace
     l = label
 
     if isinstance(func(x)[0], uncertainties.UFloat):
         if sigmas > 0:
             (ll,) = plt_plt(
-                x, unv(func(x)), fmt, label=None, color=color, linestyle=linestyle
+                x, unv(func(x)), fmt, label=None, color=color, linestyle=linestyle,**kwargs
             )
             y = func(x)
             plt.fill_between(
                 x,
                 unv(y) - sigmas * usd(y),
                 unv(y) + sigmas * usd(y),
                 alpha=alpha,
                 label=l,
                 color=ll.get_color(),
                 hatch=hatch,
+                **kwargs
             )
         else:
             (ll,) = plt_plt(
-                x, unv(func(x)), fmt, label=l, color=color, linestyle=linestyle
+                x, unv(func(x)), fmt, label=l, color=color, linestyle=linestyle,**kwargs
             )
     else:
-        (ll,) = plt_plt(x, func(x), fmt, label=l, color=color, linestyle=linestyle)
+        (ll,) = plt_plt(x, func(x), fmt, label=l, color=color, linestyle=linestyle,**kwargs)
     return ll
 
 
 def function(func, *args, **kwargs):
     """
     Plot function ``func`` between ``xmin`` and ``xmax``
 
@@ -693,30 +715,35 @@
             l = l + " " + kwargs["units"][i - 1]
     return l
 
 
 def plt_fit_or_interpolate(
     datax, datay, fitted, l=None, c=None, f=None, ls=None, **kwargs
 ):
+    # just filter these kwargs out, so they dont get passed down and are replaced by above args
+    # TODO why not pass label=XXX directly to this?
+    #      -> probably since there are cases where both e.g. color and replace color are needed
+    for key in ['color', 'label', 'fmt', 'linestyle', 'hatch']:
+        if key in kwargs:
+            del kwargs[key]
     if kwargs["prange"] is None:
         x, _, _, _ = ffit.fit_split(datax, datay, **kwargs)
         xfit = kwargs["xspace"](np.min(unv(x)), np.max(unv(x)), kwargs["steps"])
     else:
         xfit = kwargs["xspace"](
             kwargs["prange"][0], kwargs["prange"][1], kwargs["steps"]
         )
     ll = __function(
         fitted,
         xfit,
         kwargs["fit_fmt"] if f is not None and ls is None else f,
         label=l,
         color=kwargs["fit_color"] if c is None else c,
-        sigmas=kwargs["sigmas"],
         linestyle=ls,
-        alpha=kwargs["alpha"],
+        **kwargs
     )
 
     if (
         (kwargs["frange"] is not None or kwargs["fselector"] is not None)
         and util.true("extrapolate", kwargs)
         or util.has("extrapolate_max", kwargs)
         or util.has("extrapolate_min", kwargs)
@@ -732,16 +759,15 @@
         ]:
             __function(
                 fitted,
                 kwargs["xspace"](pmin, pmax, kwargs["steps"]),
                 util.get("extrapolate_fmt", kwargs, "--"),
                 color=ll.get_color(),
                 hatch=util.get("extrapolate_hatch", kwargs, r"||"),
-                sigmas=kwargs["sigmas"],
-                alpha=kwargs["alpha"],
+                **kwargs
             )
     return ll.get_color(), xfit, fitted(xfit)
 
 
 def plt_interpolate(datax, datay, icolor=None, **kwargs):
     """
     Interpolate and Plot that Interpolation.
@@ -756,25 +782,29 @@
         kargs["l"] = kwargs["interpolate_label"]
     # l = None so that no label
     return (
         inter,
         *plt_fit_or_interpolate(datax, datay, inter, c=icolor, **kargs, **kwargs),
     )
 
-
 def plt_fit(datax, datay, gfunction, **kwargs):
     """
     Fit and Plot that Fit.
     """
     func = wrap.get_lambda(gfunction, kwargs["xvar"])
     rfit = _fit(datax, datay, gfunction, **kwargs)
 
     def fitted(x):
         return func(x, *rfit)
 
+    vnames = wrap.get_varnames(gfunction, kwargs["xvar"])
+    for v in vnames[1:]: # remove fixed parameters from kwargs
+        if v in kwargs:
+            del kwargs[v]
+
     l = get_fnc_legend(gfunction, rfit, **kwargs)
     return (rfit, *plt_fit_or_interpolate(datax, datay, fitted, l, **kwargs))
 
 
 def init_plot(kwargs):
     fig = None
     if util.has("axes", kwargs) and kwargs["axes"] is not None:
```

### Comparing `smpl-1.2.5/smpl/plot2d.py` & `smpl-1.3.0/smpl/plot2d.py`

 * *Files identical despite different names*

### Comparing `smpl-1.2.5/smpl/stat.py` & `smpl-1.3.0/smpl/stat.py`

 * *Files identical despite different names*

### Comparing `smpl-1.2.5/smpl/wrap.py` & `smpl-1.3.0/smpl/wrap.py`

 * *Files identical despite different names*

### Comparing `smpl-1.2.5/setup.py` & `smpl-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'uncertainties']
 
 extras_require = \
 {'opt': ['iminuit']}
 
 setup_kwargs = {
     'name': 'smpl',
-    'version': '1.2.5',
+    'version': '1.3.0',
     'description': 'SiMPLe plotting and fitting',
     'long_description': '# smpl\nSimplified plotting and fitting in python.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/smpl.svg)\n\n| [Stable][doc stable]        | [Test][doc test]           |\n| ------------- |:-------------:|\n| [![workflow][a s image]][a s link]   | [![test][a t image]][a t link]     |\n| [![Coverage Status][c s i]][c s l]   | [![Coverage Status][c t i]][c t l] |\n| [![Codacy Badge][cc s c i]][cc s c l] | [![Codacy Badge][cc c i]][cc c l]  |\n| [![Codacy Badge][cc s q i]][cc s q l] | [![Codacy Badge][cc q i]][cc q l]  |\n| [![Documentation][rtd s i]][rtd s l] | [![Documentation][rtd t i]][rtd t l]|\n\n## Documentation\n\n-   <https://smpl.readthedocs.io/en/stable/>\n-   <https://apn-pucky.github.io/smpl/index.html>\n\n## Versions\n\n### Stable\n\n```sh\npip install smpl\n```\n\nOptional: --user or --upgrade\n\n### Dev\n\n```sh\npip install --index-url https://test.pypi.org/simple/ smpl\n```\n\n[doc stable]: https://apn-pucky.github.io/smpl/index.html\n[doc test]: https://apn-pucky.github.io/smpl/test/index.html\n\n[pypi image]: https://badge.fury.io/py/smpl.svg\n[pypi link]: https://pypi.org/project/smpl/\n[pypi versions]: https://img.shields.io/pypi/pyversions/smpl.svg\n\n[a s image]: https://github.com/APN-Pucky/smpl/actions/workflows/stable.yml/badge.svg\n[a s link]: https://github.com/APN-Pucky/smpl/actions/workflows/stable.yml\n[a t link]: https://github.com/APN-Pucky/smpl/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/smpl/actions/workflows/test.yml/badge.svg\n\n[cc s q i]: https://app.codacy.com/project/badge/Grade/38630d0063814027bd4d0ffaa73790a2?branch=stable\n[cc s q l]: https://www.codacy.com/gh/APN-Pucky/smpl/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/smpl&amp;utm_campaign=Badge_Grade?branch=stable\n[cc s c i]: https://app.codacy.com/project/badge/Coverage/38630d0063814027bd4d0ffaa73790a2?branch=stable\n[cc s c l]: https://www.codacy.com/gh/APN-Pucky/smpl/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/smpl&utm_campaign=Badge_Coverage?branch=stable\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/38630d0063814027bd4d0ffaa73790a2\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/smpl/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/smpl&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/38630d0063814027bd4d0ffaa73790a2\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/smpl/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/smpl&utm_campaign=Badge_Coverage\n\n[c s i]: https://coveralls.io/repos/github/APN-Pucky/smpl/badge.svg?branch=stable\n[c s l]: https://coveralls.io/github/APN-Pucky/smpl?branch=stable\n[c t l]: https://coveralls.io/github/APN-Pucky/smpl?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/smpl/badge.svg?branch=master\n\n[rtd s i]: https://readthedocs.org/projects/smpl/badge/?version=stable\n[rtd s l]: https://smpl.readthedocs.io/en/stable/?badge=stable\n[rtd t i]: https://readthedocs.org/projects/smpl/badge/?version=latest\n[rtd t l]: https://smpl.readthedocs.io/en/latest/?badge=latest\n',
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/smpl',
```

### Comparing `smpl-1.2.5/PKG-INFO` & `smpl-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smpl
-Version: 1.2.5
+Version: 1.3.0
 Summary: SiMPLe plotting and fitting
 Home-page: https://github.com/APN-Pucky/smpl
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

