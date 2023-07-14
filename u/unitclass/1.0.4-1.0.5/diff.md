# Comparing `tmp/unitclass-1.0.4.tar.gz` & `tmp/unitclass-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitclass-1.0.4.tar", last modified: Thu Jul 13 02:30:00 2023, max compression
+gzip compressed data, was "unitclass-1.0.5.tar", last modified: Fri Jul 14 02:31:42 2023, max compression
```

## Comparing `unitclass-1.0.4.tar` & `unitclass-1.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-13 02:30:00.131321 unitclass-1.0.4/
--rw-r--r--   0 blake      (501) staff       (20)    35149 2023-01-29 20:27:25.000000 unitclass-1.0.4/LICENSE
--rw-r--r--   0 blake      (501) staff       (20)     7282 2023-07-13 02:30:00.131186 unitclass-1.0.4/PKG-INFO
--rw-r--r--   0 blake      (501) staff       (20)     6513 2023-03-20 22:39:31.000000 unitclass-1.0.4/README.md
--rw-r--r--   0 blake      (501) staff       (20)      852 2023-07-13 02:29:51.000000 unitclass-1.0.4/pyproject.toml
--rw-r--r--   0 blake      (501) staff       (20)       38 2023-07-13 02:30:00.131354 unitclass-1.0.4/setup.cfg
-drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-13 02:30:00.131031 unitclass-1.0.4/unitclass.egg-info/
--rw-r--r--   0 blake      (501) staff       (20)     7282 2023-07-13 02:30:00.000000 unitclass-1.0.4/unitclass.egg-info/PKG-INFO
--rw-r--r--   0 blake      (501) staff       (20)      177 2023-07-13 02:30:00.000000 unitclass-1.0.4/unitclass.egg-info/SOURCES.txt
--rw-r--r--   0 blake      (501) staff       (20)        1 2023-07-13 02:30:00.000000 unitclass-1.0.4/unitclass.egg-info/dependency_links.txt
--rw-r--r--   0 blake      (501) staff       (20)       10 2023-07-13 02:30:00.000000 unitclass-1.0.4/unitclass.egg-info/top_level.txt
--rw-r--r--   0 blake      (501) staff       (20)    43370 2023-07-13 02:29:37.000000 unitclass-1.0.4/unitclass.py
+drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-14 02:31:42.877619 unitclass-1.0.5/
+-rw-r--r--   0 blake      (501) staff       (20)    35149 2023-01-29 20:27:25.000000 unitclass-1.0.5/LICENSE
+-rw-r--r--   0 blake      (501) staff       (20)     7282 2023-07-14 02:31:42.877475 unitclass-1.0.5/PKG-INFO
+-rw-r--r--   0 blake      (501) staff       (20)     6513 2023-03-20 22:39:31.000000 unitclass-1.0.5/README.md
+-rw-r--r--   0 blake      (501) staff       (20)      852 2023-07-14 02:31:00.000000 unitclass-1.0.5/pyproject.toml
+-rw-r--r--   0 blake      (501) staff       (20)       38 2023-07-14 02:31:42.877661 unitclass-1.0.5/setup.cfg
+drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-14 02:31:42.877283 unitclass-1.0.5/unitclass.egg-info/
+-rw-r--r--   0 blake      (501) staff       (20)     7282 2023-07-14 02:31:42.000000 unitclass-1.0.5/unitclass.egg-info/PKG-INFO
+-rw-r--r--   0 blake      (501) staff       (20)      177 2023-07-14 02:31:42.000000 unitclass-1.0.5/unitclass.egg-info/SOURCES.txt
+-rw-r--r--   0 blake      (501) staff       (20)        1 2023-07-14 02:31:42.000000 unitclass-1.0.5/unitclass.egg-info/dependency_links.txt
+-rw-r--r--   0 blake      (501) staff       (20)       10 2023-07-14 02:31:42.000000 unitclass-1.0.5/unitclass.egg-info/top_level.txt
+-rw-r--r--   0 blake      (501) staff       (20)    43608 2023-07-14 02:30:50.000000 unitclass-1.0.5/unitclass.py
```

### Comparing `unitclass-1.0.4/LICENSE` & `unitclass-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `unitclass-1.0.4/PKG-INFO` & `unitclass-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitclass
-Version: 1.0.4
+Version: 1.0.5
 Summary: Physical unit class suitable for calculations in the sciences.
 Author-email: Blake Garretson <blake@blakeg.net>
 Project-URL: Homepage, https://github.com/blakegarretson/unitclass
 Project-URL: Bug Tracker, https://github.com/blakegarretson/unitclass/issues
 Keywords: unit,units,SI,conversion
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `unitclass-1.0.4/README.md` & `unitclass-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `unitclass-1.0.4/pyproject.toml` & `unitclass-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unitclass"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Blake Garretson", email="blake@blakeg.net" },
 ]
 description = "Physical unit class suitable for calculations in the sciences."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `unitclass-1.0.4/unitclass.egg-info/PKG-INFO` & `unitclass-1.0.5/unitclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitclass
-Version: 1.0.4
+Version: 1.0.5
 Summary: Physical unit class suitable for calculations in the sciences.
 Author-email: Blake Garretson <blake@blakeg.net>
 Project-URL: Homepage, https://github.com/blakegarretson/unitclass
 Project-URL: Bug Tracker, https://github.com/blakegarretson/unitclass/issues
 Keywords: unit,units,SI,conversion
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `unitclass-1.0.4/unitclass.py` & `unitclass-1.0.5/unitclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,35 +171,39 @@
     ('solid_angle', 'sr', 'steradian', 1, ''),
     ('dose_equivalent', 'Sv', 'sievert sieverts', 1, ''),
     ('conductance', 'S', 'siemens', 1, ''),
     ('angle', 'rad', 'rads radians radian', 1, ''),
     # Other units below
     ('unitless', '', 'unitless _', 1, ''),
     ('time', 'min', 'minute minutes', 60, 's'),
-    ('time', 'hr', 'hour hours', 60, 'min'),
+    ('time', 'hr', 'hrs hour hours', 60, 'min'),
     ('time', 'day', 'days', 24, 'hr'),
     ('time', 'week', 'weeks', 7, 'day'),
     ('time', 'fortnight', 'fortnights', 14, 'day'),
     ('time', 'year', 'yr yrs years', 365, 'day'),
     ('length', 'in', 'inch inches "', 25.4, 'mm'),
     ('length', 'ft', "feet ' foot", 12, 'in'),
     ('length', 'yd', 'yard yards', 36, 'in'),
     ('length', 'mi', 'mile miles statutemile statutemiles smi', 5280, 'ft'),
     ('length', 'nmi', 'nauticalmile nauticalmiles', 1852, 'm'),
+    ('length', 'league_land', 'leagues_land', 3, 'mi'),
+    ('length', 'league_sea', 'leagues_sea nauticalleague nauticalleagues', 3, 'nmi'),
     ('length', 'gmi', 'geographicalmile geographicalmiles', 1855.3247, 'm'),
     ('length', 'mil', '', 0.001, 'in'),
     ('length', 'thou', '', 0.001, 'in'),
     ('length', 'micron', 'microns', 1, 'um'),
     ('length', 'cl', 'caliber', 1, 'in'),
     ('length', 'pt', 'point points pts', 1 / 72, 'in'),
     ('length', 'pica', 'picas', 12, 'pt'),
     ('length', 'angstrom', 'ang', 0.1, 'nm'),
     ('length', 'furlong', 'furlongs', 660, 'ft'),
     ('length', 'intl_cable', 'intl_cables', 185.2, 'm'),
     ('length', 'imp_cable', 'imp_cables', 185.32, 'm'),
+    ('length', 'chain', 'chains', 66, 'ft'),
+    ('length', 'link', 'links', 100, 'chain'),
     ('length', 'us_cable', 'us_cables', 720, 'ft'),
     ('length', 'fathom', 'fathoms', 6, 'ft'),
     ('length', 'hand', 'hands', 4, 'in'),
     ('length', 'bohrrad', 'bohrradius', 5.29177210903e-11, 'm'),
     ('length', 'smoot', 'smoots', 67, 'in'),
     ('length', 'au', 'astrounit', 149597870.691, 'km'),
     ('acceleration', 'G', 'gravity', g, 'm/s2'),
```

