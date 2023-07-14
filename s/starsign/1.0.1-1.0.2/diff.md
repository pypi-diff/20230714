# Comparing `tmp/starsign-1.0.1.tar.gz` & `tmp/starsign-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starsign-1.0.1.tar", last modified: Fri Jul 14 14:17:15 2023, max compression
+gzip compressed data, was "dist/starsign-1.0.2.tar", last modified: Fri Jul 14 16:52:07 2023, max compression
```

## Comparing `starsign-1.0.1.tar` & `starsign-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 theo      (1001) theo      (1001)        0 2023-07-14 14:17:15.960783 starsign-1.0.1/
--rw-rw-r--   0 theo      (1001) theo      (1001)     1082 2023-07-14 04:04:26.000000 starsign-1.0.1/LICENSE
--rw-rw-r--   0 theo      (1001) theo      (1001)      214 2023-07-14 14:17:15.960783 starsign-1.0.1/PKG-INFO
--rw-rw-r--   0 theo      (1001) theo      (1001)     1073 2023-07-14 13:30:50.000000 starsign-1.0.1/README.md
--rw-rw-r--   0 theo      (1001) theo      (1001)       38 2023-07-14 14:17:15.960783 starsign-1.0.1/setup.cfg
--rw-rw-r--   0 theo      (1001) theo      (1001)      680 2023-07-14 04:04:26.000000 starsign-1.0.1/setup.py
-drwxrwxr-x   0 theo      (1001) theo      (1001)        0 2023-07-14 14:17:15.960783 starsign-1.0.1/starsign/
--rw-rw-r--   0 theo      (1001) theo      (1001)       34 2023-07-14 14:13:30.000000 starsign-1.0.1/starsign/__init__.py
--rw-rw-r--   0 theo      (1001) theo      (1001)     7894 2023-07-14 04:04:26.000000 starsign-1.0.1/starsign/starsign.py
--rw-rw-r--   0 theo      (1001) theo      (1001)     2729 2023-07-14 04:04:26.000000 starsign-1.0.1/starsign/test_suite.py
-drwxrwxr-x   0 theo      (1001) theo      (1001)        0 2023-07-14 14:17:15.960783 starsign-1.0.1/starsign.egg-info/
--rw-rw-r--   0 theo      (1001) theo      (1001)      214 2023-07-14 14:17:15.000000 starsign-1.0.1/starsign.egg-info/PKG-INFO
--rw-rw-r--   0 theo      (1001) theo      (1001)      250 2023-07-14 14:17:15.000000 starsign-1.0.1/starsign.egg-info/SOURCES.txt
--rw-rw-r--   0 theo      (1001) theo      (1001)        1 2023-07-14 14:17:15.000000 starsign-1.0.1/starsign.egg-info/dependency_links.txt
--rw-rw-r--   0 theo      (1001) theo      (1001)       65 2023-07-14 14:17:15.000000 starsign-1.0.1/starsign.egg-info/requires.txt
--rw-rw-r--   0 theo      (1001) theo      (1001)        9 2023-07-14 14:17:15.000000 starsign-1.0.1/starsign.egg-info/top_level.txt
+drwxrwxr-x   0 theo      (1001) theo      (1001)        0 2023-07-14 16:52:07.000000 starsign-1.0.2/
+-rw-rw-r--   0 theo      (1001) theo      (1001)     1082 2023-07-14 04:04:26.000000 starsign-1.0.2/LICENSE
+-rw-rw-r--   0 theo      (1001) theo      (1001)      214 2023-07-14 16:52:07.000000 starsign-1.0.2/PKG-INFO
+-rw-rw-r--   0 theo      (1001) theo      (1001)     1354 2023-07-14 16:50:05.000000 starsign-1.0.2/README.md
+-rw-rw-r--   0 theo      (1001) theo      (1001)       38 2023-07-14 16:52:07.000000 starsign-1.0.2/setup.cfg
+-rw-rw-r--   0 theo      (1001) theo      (1001)      680 2023-07-14 04:04:26.000000 starsign-1.0.2/setup.py
+drwxrwxr-x   0 theo      (1001) theo      (1001)        0 2023-07-14 16:52:07.000000 starsign-1.0.2/starsign/
+-rw-rw-r--   0 theo      (1001) theo      (1001)       34 2023-07-14 16:50:56.000000 starsign-1.0.2/starsign/__init__.py
+-rw-rw-r--   0 theo      (1001) theo      (1001)     7909 2023-07-14 16:50:05.000000 starsign-1.0.2/starsign/starsign.py
+-rw-rw-r--   0 theo      (1001) theo      (1001)     2729 2023-07-14 04:04:26.000000 starsign-1.0.2/starsign/test_suite.py
+drwxrwxr-x   0 theo      (1001) theo      (1001)        0 2023-07-14 16:52:07.000000 starsign-1.0.2/starsign.egg-info/
+-rw-rw-r--   0 theo      (1001) theo      (1001)      214 2023-07-14 16:52:07.000000 starsign-1.0.2/starsign.egg-info/PKG-INFO
+-rw-rw-r--   0 theo      (1001) theo      (1001)      250 2023-07-14 16:52:07.000000 starsign-1.0.2/starsign.egg-info/SOURCES.txt
+-rw-rw-r--   0 theo      (1001) theo      (1001)        1 2023-07-14 16:52:07.000000 starsign-1.0.2/starsign.egg-info/dependency_links.txt
+-rw-rw-r--   0 theo      (1001) theo      (1001)       65 2023-07-14 16:52:07.000000 starsign-1.0.2/starsign.egg-info/requires.txt
+-rw-rw-r--   0 theo      (1001) theo      (1001)        9 2023-07-14 16:52:07.000000 starsign-1.0.2/starsign.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `starsign-1.0.1/LICENSE` & `starsign-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `starsign-1.0.1/README.md` & `starsign-1.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+[![A rectangular badge, half black half purple containing the text made at Code Astro](https://img.shields.io/badge/Made%20at-Code/Astro-blueviolet.svg)](https://semaphorep.github.io/codeastro/)
 # starsign
 
 Given an Earth location, date, and time, this package can find the star closest to directly overhead. If you want a horoscope backed by the full might of SIMBAD, then it's your lucky day!
 
 **Example usage:**
 ```
 from starsign.starsign import StarSign
@@ -17,12 +18,12 @@
 print(s.star['OTYPE'])
 HighPM*
 ```
 The object and surrounding area can be visualized by running:
 ```
 s.visualize()
 ```
-For more details on functionality, run help(StarSign) from within a Python session. This software package can be installed by running:
+For more details on functionality, visit [our ReadTheDocs page](https://starsign.readthedocs.io/en/latest/index.html) or run help(StarSign) from within a Python session. This software package can be installed by running:
 ```
 pip install starsign
 ```
 from a terminal window or downloaded from [our PyPI page](https://pypi.org/project/starsign/).
```

### Comparing `starsign-1.0.1/setup.py` & `starsign-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `starsign-1.0.1/starsign/starsign.py` & `starsign-1.0.2/starsign/starsign.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                                          ra,dec,fov)
             except(AttributeError):
                 result = hips2fits.query('Gaia DR3',width,height,'TAN',
                                          ra,dec,fov)
         except:
             raise RuntimeError('Read from HiPS timed out; try fewer pixels')
                 
-        im = plt.imshow(result[0].data,cmap=cmap)
+        im = plt.imshow(result[0].data,cmap=cmap,origin='lower')
 
         #handle display of coordinates for different widths and heights
         min_px,max_px = min(width,height),max(width,height)
         ticks = np.linspace(.25,.75,3)*max_px
         short_ticks = np.linspace(min(ticks),max(ticks),len(ticks))-(max_px-min_px)/2
         short_ticks = short_ticks[np.logical_and(short_ticks > 0,short_ticks < min_px)]
         tick_scale = np.format_float_positional(fov.value/4,precision=3)
```

### Comparing `starsign-1.0.1/starsign/test_suite.py` & `starsign-1.0.2/starsign/test_suite.py`

 * *Files identical despite different names*

