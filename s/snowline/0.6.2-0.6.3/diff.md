# Comparing `tmp/snowline-0.6.2.tar.gz` & `tmp/snowline-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowline-0.6.2.tar", last modified: Tue Sep 13 14:39:58 2022, max compression
+gzip compressed data, was "snowline-0.6.3.tar", last modified: Fri Jul 14 08:31:22 2023, max compression
```

## Comparing `snowline-0.6.2.tar` & `snowline-0.6.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2022-09-13 14:39:58.467057 snowline-0.6.2/
--rw-r--r--   0 user      (1000) jbuchner  (1000)     3544 2021-02-04 15:32:31.000000 snowline-0.6.2/CONTRIBUTING.rst
--rw-r--r--   0 user      (1000) jbuchner  (1000)      361 2021-02-04 15:32:31.000000 snowline-0.6.2/HISTORY.rst
--rw-r--r--   0 user      (1000) jbuchner  (1000)     1597 2021-02-04 15:32:31.000000 snowline-0.6.2/LICENSE
--rw-r--r--   0 user      (1000) jbuchner  (1000)      242 2021-02-04 15:32:31.000000 snowline-0.6.2/MANIFEST.in
--rw-r--r--   0 user      (1000) jbuchner  (1000)     3183 2022-09-13 14:39:58.467057 snowline-0.6.2/PKG-INFO
--rw-r--r--   0 user      (1000) jbuchner  (1000)     1858 2021-07-08 08:56:02.000000 snowline-0.6.2/README.rst
-drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2022-09-13 14:39:58.463057 snowline-0.6.2/docs/
--rw-r--r--   0 user      (1000) jbuchner  (1000)      606 2021-02-04 15:32:31.000000 snowline-0.6.2/docs/Makefile
--rwxr-xr-x   0 user      (1000) jbuchner  (1000)     5898 2021-02-04 15:32:31.000000 snowline-0.6.2/docs/conf.py
--rw-r--r--   0 user      (1000) jbuchner  (1000)       33 2021-02-04 15:32:31.000000 snowline-0.6.2/docs/contributing.rst
--rw-r--r--   0 user      (1000) jbuchner  (1000)       28 2021-02-04 15:32:31.000000 snowline-0.6.2/docs/history.rst
--rw-r--r--   0 user      (1000) jbuchner  (1000)      340 2021-02-04 15:32:31.000000 snowline-0.6.2/docs/index.rst
--rw-r--r--   0 user      (1000) jbuchner  (1000)     1423 2021-02-04 15:32:31.000000 snowline-0.6.2/docs/installation.rst
--rw-r--r--   0 user      (1000) jbuchner  (1000)      615 2021-02-04 15:32:31.000000 snowline-0.6.2/docs/issues.rst
--rw-r--r--   0 user      (1000) jbuchner  (1000)      769 2021-02-04 15:32:31.000000 snowline-0.6.2/docs/make.bat
--rw-r--r--   0 user      (1000) jbuchner  (1000)       51 2021-02-04 15:32:31.000000 snowline-0.6.2/docs/modules.rst
--rw-r--r--   0 user      (1000) jbuchner  (1000)       27 2021-02-04 15:32:31.000000 snowline-0.6.2/docs/readme.rst
--rw-r--r--   0 user      (1000) jbuchner  (1000)      112 2021-02-04 15:32:31.000000 snowline-0.6.2/docs/snowline.rst
--rw-r--r--   0 user      (1000) jbuchner  (1000)      455 2022-09-13 14:39:58.467057 snowline-0.6.2/setup.cfg
--rw-r--r--   0 user      (1000) jbuchner  (1000)     1894 2022-09-13 14:39:57.000000 snowline-0.6.2/setup.py
-drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2022-09-13 14:39:58.467057 snowline-0.6.2/snowline.egg-info/
--rw-r--r--   0 user      (1000) jbuchner  (1000)     3183 2022-09-13 14:39:58.000000 snowline-0.6.2/snowline.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) jbuchner  (1000)      451 2022-09-13 14:39:58.000000 snowline-0.6.2/snowline.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) jbuchner  (1000)        1 2022-09-13 14:39:58.000000 snowline-0.6.2/snowline.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) jbuchner  (1000)       26 2022-09-13 14:39:58.000000 snowline-0.6.2/snowline.egg-info/requires.txt
--rw-r--r--   0 user      (1000) jbuchner  (1000)        9 2022-09-13 14:39:58.000000 snowline-0.6.2/snowline.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) jbuchner  (1000)    32826 2022-09-13 14:39:57.000000 snowline-0.6.2/snowline.py
-drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2022-09-13 14:39:58.467057 snowline-0.6.2/tests/
--rw-r--r--   0 user      (1000) jbuchner  (1000)     4018 2022-04-24 08:41:09.000000 snowline-0.6.2/tests/test_run.py
+drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2023-07-14 08:31:22.781370 snowline-0.6.3/
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     3544 2021-02-04 15:32:31.000000 snowline-0.6.3/CONTRIBUTING.rst
+-rw-r--r--   0 user      (1000) jbuchner  (1000)      361 2021-02-04 15:32:31.000000 snowline-0.6.3/HISTORY.rst
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     1597 2021-02-04 15:32:31.000000 snowline-0.6.3/LICENSE
+-rw-r--r--   0 user      (1000) jbuchner  (1000)      242 2021-02-04 15:32:31.000000 snowline-0.6.3/MANIFEST.in
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     3184 2023-07-14 08:31:22.781370 snowline-0.6.3/PKG-INFO
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     1858 2021-07-08 08:56:02.000000 snowline-0.6.3/README.rst
+drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2023-07-14 08:31:22.777370 snowline-0.6.3/docs/
+-rw-r--r--   0 user      (1000) jbuchner  (1000)      606 2021-02-04 15:32:31.000000 snowline-0.6.3/docs/Makefile
+-rwxr-xr-x   0 user      (1000) jbuchner  (1000)     5898 2021-02-04 15:32:31.000000 snowline-0.6.3/docs/conf.py
+-rw-r--r--   0 user      (1000) jbuchner  (1000)       33 2021-02-04 15:32:31.000000 snowline-0.6.3/docs/contributing.rst
+-rw-r--r--   0 user      (1000) jbuchner  (1000)       28 2021-02-04 15:32:31.000000 snowline-0.6.3/docs/history.rst
+-rw-r--r--   0 user      (1000) jbuchner  (1000)      340 2021-02-04 15:32:31.000000 snowline-0.6.3/docs/index.rst
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     1423 2021-02-04 15:32:31.000000 snowline-0.6.3/docs/installation.rst
+-rw-r--r--   0 user      (1000) jbuchner  (1000)      615 2021-02-04 15:32:31.000000 snowline-0.6.3/docs/issues.rst
+-rw-r--r--   0 user      (1000) jbuchner  (1000)      769 2021-02-04 15:32:31.000000 snowline-0.6.3/docs/make.bat
+-rw-r--r--   0 user      (1000) jbuchner  (1000)       51 2021-02-04 15:32:31.000000 snowline-0.6.3/docs/modules.rst
+-rw-r--r--   0 user      (1000) jbuchner  (1000)       27 2021-02-04 15:32:31.000000 snowline-0.6.3/docs/readme.rst
+-rw-r--r--   0 user      (1000) jbuchner  (1000)      112 2021-02-04 15:32:31.000000 snowline-0.6.3/docs/snowline.rst
+-rw-r--r--   0 user      (1000) jbuchner  (1000)      455 2023-07-14 08:31:22.781370 snowline-0.6.3/setup.cfg
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     1950 2023-07-14 08:31:17.000000 snowline-0.6.3/setup.py
+drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2023-07-14 08:31:22.781370 snowline-0.6.3/snowline.egg-info/
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     3184 2023-07-14 08:31:22.000000 snowline-0.6.3/snowline.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) jbuchner  (1000)      451 2023-07-14 08:31:22.000000 snowline-0.6.3/snowline.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) jbuchner  (1000)        1 2023-07-14 08:31:22.000000 snowline-0.6.3/snowline.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) jbuchner  (1000)       52 2023-07-14 08:31:22.000000 snowline-0.6.3/snowline.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) jbuchner  (1000)        9 2023-07-14 08:31:22.000000 snowline-0.6.3/snowline.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) jbuchner  (1000)    32864 2023-07-14 08:31:17.000000 snowline-0.6.3/snowline.py
+drwxr-xr-x   0 user      (1000) jbuchner  (1000)        0 2023-07-14 08:31:22.781370 snowline-0.6.3/tests/
+-rw-r--r--   0 user      (1000) jbuchner  (1000)     4018 2022-04-24 08:41:09.000000 snowline-0.6.3/tests/test_run.py
```

### Comparing `snowline-0.6.2/CONTRIBUTING.rst` & `snowline-0.6.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `snowline-0.6.2/LICENSE` & `snowline-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `snowline-0.6.2/PKG-INFO` & `snowline-0.6.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: snowline
-Version: 0.6.2
+Version: 0.6.3
 Summary: Fit and compare complex models quickly. Laplace Approximation, Variational Bayes, Importance Sampling.
 Home-page: https://github.com/JohannesBuchner/snowline
 Author: Johannes Buchner
 Author-email: johannes.buchner.acad@gmx.com
 License: GNU General Public License v3
 Keywords: snowline
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
+Provides-Extra: plot
 License-File: LICENSE
 
 =========
 snowline
 =========
 
 Fit and compare models very quickly. MCMC-free.
@@ -113,9 +113,7 @@
 * Packaging and testing improvements
 
 
 0.1.0 (2020-03-07)
 ------------------
 
 * First version
-
-
```

### Comparing `snowline-0.6.2/README.rst` & `snowline-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `snowline-0.6.2/docs/Makefile` & `snowline-0.6.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `snowline-0.6.2/docs/conf.py` & `snowline-0.6.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `snowline-0.6.2/docs/installation.rst` & `snowline-0.6.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `snowline-0.6.2/docs/issues.rst` & `snowline-0.6.3/docs/issues.rst`

 * *Files identical despite different names*

### Comparing `snowline-0.6.2/docs/make.bat` & `snowline-0.6.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `snowline-0.6.2/setup.py` & `snowline-0.6.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,10 +48,11 @@
     long_description=readme + '\n\n' + history,
     keywords='snowline',
     name='snowline',
     py_modules=['snowline'],
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
+    extras_require=dict(plot=['matplotlib', 'corner']),
     url='https://github.com/JohannesBuchner/snowline',
-    version='0.6.2',
+    version='0.6.3',
 )
```

### Comparing `snowline-0.6.2/snowline.egg-info/PKG-INFO` & `snowline-0.6.3/snowline.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: snowline
-Version: 0.6.2
+Version: 0.6.3
 Summary: Fit and compare complex models quickly. Laplace Approximation, Variational Bayes, Importance Sampling.
 Home-page: https://github.com/JohannesBuchner/snowline
 Author: Johannes Buchner
 Author-email: johannes.buchner.acad@gmx.com
 License: GNU General Public License v3
 Keywords: snowline
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
+Provides-Extra: plot
 License-File: LICENSE
 
 =========
 snowline
 =========
 
 Fit and compare models very quickly. MCMC-free.
@@ -113,9 +113,7 @@
 * Packaging and testing improvements
 
 
 0.1.0 (2020-03-07)
 ------------------
 
 * First version
-
-
```

### Comparing `snowline-0.6.2/snowline.py` & `snowline-0.6.3/snowline.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from pypmc.tools.convergence import ess
 from pypmc.mix_adapt.variational import GaussianInference
 
 
 __all__ = ['ReactiveImportanceSampler']
 __author__ = """Johannes Buchner"""
 __email__ = 'johannes.buchner.acad@gmx.com'
-__version__ = '0.6.2'
+__version__ = '0.6.3'
 
 
 # Some parts are from the nnest library by Adam Moss (https://github.com/adammoss/nnest)
 def create_logger(module_name, log_dir=None, level=logging.INFO):
     """
     Set up the logging channel `module_name`.
 
@@ -121,15 +121,15 @@
 
     if N is None:
         N = len(weights)
 
     # make N subdivisions, and choose positions with a consistent random offset
     positions = (rstate.random() + np.arange(N)) / N
 
-    idx = np.zeros(N, dtype=np.int)
+    idx = np.zeros(N, dtype=int)
     cumulative_sum = np.cumsum(weights)
     i, j = 0, 0
     while i < N:
         if positions[i] < cumulative_sum[j]:
             idx[i] = j
             i += 1
         else:
@@ -627,17 +627,16 @@
 
             def negloglike(u):
                 """ negative log-likelihood to minimize """
                 p = self.transform(u)
                 return -self.loglike(p)
 
             if self.log:
-                self.logger.debug("    starting optimization...")
-                self.logger.info("    from: %s" % startu)
-                self.logger.info("    error: %s" % deltau)
+                self.logger.info("    starting optimization from: %s", startu)
+                self.logger.info("    error: %s", deltau)
             if hasattr(Minuit, 'from_array_func'):
                 m = Minuit.from_array_func(
                     negloglike, startu, errordef=0.5,
                     error=deltau, limit=[(0, 1)] * ndim)
             else:
                 m = Minuit(negloglike, startu)
                 m.errordef = Minuit.LIKELIHOOD
@@ -654,14 +653,15 @@
             optu = [max(1e-10, min(1 - 1e-10, m.values[i])) for i in range(ndim)]
             optp = np.asarray(self.transform(np.asarray(optu)))
             umax = [max(1e-6, min(1 - 1e-6, m.values[i] + m.errors[i])) for i in range(ndim)]
             umin = [max(1e-6, min(1 - 1e-6, m.values[i] - m.errors[i])) for i in range(ndim)]
             pmax = np.asarray(self.transform(np.asarray(umax)))
             pmin = np.asarray(self.transform(np.asarray(umin)))
             perr = (pmax - pmin) / 2
+            self.logger.info("    optimization finished at L=%.1f: %s" % (optL, optp))
 
             for name, med, sigma in zip(self.paramnames, optp, perr):
                 if sigma > 0:
                     i = max(0, int(-np.floor(np.log10(sigma))) + 1)
                 else:
                     i = 3
                 fmt = '%%.%df' % i
```

### Comparing `snowline-0.6.2/tests/test_run.py` & `snowline-0.6.3/tests/test_run.py`

 * *Files identical despite different names*

