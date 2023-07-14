# Comparing `tmp/kirkwoodnight-0.9.tar.gz` & `tmp/kirkwoodnight-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kirkwoodnight-0.9.tar", last modified: Wed Jul 12 22:28:40 2023, max compression
+gzip compressed data, was "kirkwoodnight-1.0.0.tar", last modified: Fri Jul 14 03:10:06 2023, max compression
```

## Comparing `kirkwoodnight-0.9.tar` & `kirkwoodnight-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 22:28:40.072592 kirkwoodnight-0.9/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1119 2023-07-12 19:15:12.000000 kirkwoodnight-0.9/LICENSE.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)     2229 2023-07-12 22:28:40.072270 kirkwoodnight-0.9/PKG-INFO
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1768 2023-07-12 19:53:44.000000 kirkwoodnight-0.9/README.md
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 22:28:40.069408 kirkwoodnight-0.9/kirkwoodnight/
--rw-r--r--   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:58:50.000000 kirkwoodnight-0.9/kirkwoodnight/__init__.py
--rw-r--r--   0 armaangoyal   (501) staff       (20)     2746 2023-07-12 22:25:38.000000 kirkwoodnight-0.9/kirkwoodnight/command_line.py
--rw-r--r--   0 armaangoyal   (501) staff       (20)     7948 2023-07-12 14:27:02.000000 kirkwoodnight-0.9/kirkwoodnight/obj_list.csv
--rw-r--r--   0 armaangoyal   (501) staff       (20)    15900 2023-07-12 22:18:18.000000 kirkwoodnight-0.9/kirkwoodnight/source.py
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 22:28:40.071823 kirkwoodnight-0.9/kirkwoodnight.egg-info/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     2229 2023-07-12 22:28:39.000000 kirkwoodnight-0.9/kirkwoodnight.egg-info/PKG-INFO
--rw-r--r--   0 armaangoyal   (501) staff       (20)      361 2023-07-12 22:28:40.000000 kirkwoodnight-0.9/kirkwoodnight.egg-info/SOURCES.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-12 22:28:39.000000 kirkwoodnight-0.9/kirkwoodnight.egg-info/dependency_links.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       66 2023-07-12 22:28:39.000000 kirkwoodnight-0.9/kirkwoodnight.egg-info/entry_points.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       58 2023-07-12 22:28:39.000000 kirkwoodnight-0.9/kirkwoodnight.egg-info/requires.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       14 2023-07-12 22:28:39.000000 kirkwoodnight-0.9/kirkwoodnight.egg-info/top_level.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       38 2023-07-12 22:28:40.072709 kirkwoodnight-0.9/setup.cfg
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1089 2023-07-12 22:28:20.000000 kirkwoodnight-0.9/setup.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:10:06.870000 kirkwoodnight-1.0.0/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1119 2023-07-12 19:15:12.000000 kirkwoodnight-1.0.0/LICENSE.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     5023 2023-07-14 03:10:06.869439 kirkwoodnight-1.0.0/PKG-INFO
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     4560 2023-07-13 00:00:36.000000 kirkwoodnight-1.0.0/README.md
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:10:06.860569 kirkwoodnight-1.0.0/kirkwoodnight/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:58:50.000000 kirkwoodnight-1.0.0/kirkwoodnight/__init__.py
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     4304 2023-07-14 02:42:02.000000 kirkwoodnight-1.0.0/kirkwoodnight/command_line.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:10:06.868528 kirkwoodnight-1.0.0/kirkwoodnight/data/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     7833 2023-07-13 23:53:52.000000 kirkwoodnight-1.0.0/kirkwoodnight/data/obj_list.csv
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     6350 2023-07-14 03:09:07.000000 kirkwoodnight-1.0.0/kirkwoodnight/plotting.py
+-rw-r--r--   0 armaangoyal   (501) staff       (20)    18480 2023-07-14 02:43:02.000000 kirkwoodnight-1.0.0/kirkwoodnight/source.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:10:06.867718 kirkwoodnight-1.0.0/kirkwoodnight.egg-info/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     5023 2023-07-14 03:10:06.000000 kirkwoodnight-1.0.0/kirkwoodnight.egg-info/PKG-INFO
+-rw-r--r--   0 armaangoyal   (501) staff       (20)      392 2023-07-14 03:10:06.000000 kirkwoodnight-1.0.0/kirkwoodnight.egg-info/SOURCES.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-14 03:10:06.000000 kirkwoodnight-1.0.0/kirkwoodnight.egg-info/dependency_links.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       66 2023-07-14 03:10:06.000000 kirkwoodnight-1.0.0/kirkwoodnight.egg-info/entry_points.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       58 2023-07-14 03:10:06.000000 kirkwoodnight-1.0.0/kirkwoodnight.egg-info/requires.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       14 2023-07-14 03:10:06.000000 kirkwoodnight-1.0.0/kirkwoodnight.egg-info/top_level.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       38 2023-07-14 03:10:06.870205 kirkwoodnight-1.0.0/setup.cfg
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1089 2023-07-14 03:09:51.000000 kirkwoodnight-1.0.0/setup.py
```

### Comparing `kirkwoodnight-0.9/LICENSE.txt` & `kirkwoodnight-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-0.9/kirkwoodnight/obj_list.csv` & `kirkwoodnight-1.0.0/kirkwoodnight/data/obj_list.csv`

 * *Files 25% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-Name,RA,Dec,Type,Constellation,Magnitude
-NGC 1952 Crab Nebula,83.625,22.01666667,Supernova Remnant,Taurus,8.4
-NGC 7089  ,323.375,-0.816666667,Globular Cluster,Aquarius,6.5
-NGC 5272  ,205.55,28.38333333,Globular Cluster,Canes Venatici,6.2
-NGC 6121  ,245.9,-26.53333333,Globular Cluster,Scorpius,5.6
-NGC 5904  ,229.65,2.083333333,Globular Cluster,Serpens Caput,5.6
-NGC 6405 Butterfly Cluster,265.025,-32.21666667,Open Cluster,Scorpius,5.3
-NGC 6475 Ptolemy¹s Cluster,268.475,-34.81666667,Open Cluster,Scorpius,4.1
-NGC 6523 Lagoon Nebula,270.95,-24.38333333,Diffuse Nebula,Sagittarius,6
-NGC 6333  ,259.8,-18.51666667,Globular Cluster,Ophiucus,7.7
-NGC 6254  ,254.275,-4.1,Globular Cluster,Ophiucus,6.6
-NGC 6705 Wild Duck Cluster,282.775,-6.266666667,Open Cluster,Scutum,6.3
-NGC 6218  ,251.8,-1.95,Globular Cluster,Ophiucus,6.7
-NGC 6205 Hercules Globular Cluster,250.425,36.46666667,Globular Cluster,Hercules,5.8
-NGC 6402  ,264.4,-3.25,Globular Cluster,Ophiucus,7.6
-NGC 7078  ,322.5,12.16666667,Globular Cluster,Pegasus,6.2
-NGC 6611 Eagle Nebula Cluster,274.7,-13.78333333,Open Cluster,Serpens Claudia,6.4
-"NGC 6618 Omega, Swan, Horseshoe Nebula",275.2,-16.18333333,Diffuse Nebula,Sagittarius,7
-NGC 6613  ,274.975,-17.13333333,Open Cluster,Sagittarius,7.5
-NGC 6273  ,255.65,-26.26666667,Globular Cluster,Ophiucus,6.8
-NGC 6514 Trifid Nebula,270.575,-23.03333333,Diffuse Nebula,Sagittarius,9
-NGC 6531  ,271.15,-22.5,Open Cluster,Sagittarius,6.5
-NGC 6656  ,279.1,-23.9,Globular Cluster,Sagittarius,5.1
-NGC 6494  ,269.2,-19.01666667,Open Cluster,Sagittarius,6.9
-NGC 6603 Milky Way Patch,274.6,-18.41666667,Star Cloud,Sagittarius,4.6
-IC 4725,277.925,-19.23333333,Open Cluster,Sagittarius,6.5
-NGC 6694  ,281.3,-9.4,Open Cluster,Scutum,8
-NGC 6853 Dumbbell Nebula,299.9,22.71666667,Planetary Nebula,Vulpecula,7.4
-NGC 6626  ,276.125,-24.86666667,Globular Cluster,Sagittarius,6.8
-NGC 6913  ,305.975,38.53333333,Open Cluster,Cygnus,7.1
-NGC 7099  ,325.1,-23.18333333,Globular Cluster,Capricornus,7.2
-NGC 224 Andromeda Galaxy,10.675,41.26666667,Spiral Galaxy,Andromeda,3.4
-NGC 221 Satellite of M31,10.675,40.86666667,Elliptical Galaxy,Andromeda,8.1
-NGC 598 Triangulum-Pinwheel Galaxy,23.475,30.65,Spiral Galaxy,Triangulum,5.7
-NGC 1039  ,40.5,42.78333333,Open Cluster,Perseus,5.5
-NGC 2168  ,92.225,24.33333333,Open Cluster,Gemini,5.3
-NGC 1960  ,84.025,34.13333333,Open Cluster,Auriga,6.3
-NGC 2099  ,88.1,32.55,Open Cluster,Auriga,6.2
-NGC 1912  ,82.175,35.83333333,Open Cluster,Auriga,7.4
-NGC 7092  ,323.05,48.43333333,Open Cluster,Cygnus,5.2
-Winecke 4,185.55,58.08333333,Double Star,Ursa Major,9.3
-NGC 2287  ,101.75,-20.73333333,Open Cluster,Canis Major,4.6
-NGC 1976 Great Orion Nebula,83.85,-5.45,Diffuse Nebula,Orion,4
-NGC 1982 de Mairan¹s Nebula,83.9,-5.266666667,Diffuse Nebula,Orion,9
-NGC 2632 Beehive Cluster (Praesepe),130.025,19.98333333,Open Cluster,Cancer,3.7
-"Pleiades, Subaru, Seven Sisters",56.75,24.12,Open Cluster,Taurus,1.6
-NGC 2437  ,115.45,-14.81666667,Open Cluster,Puppis,6
-NGC 2422  ,114.15,-14.5,Open Cluster,Puppis,5.2
-NGC 2548  ,123.45,-5.8,Open Cluster,Hydra,5.5
-NGC 4472  ,187.45,8,Elliptical Galaxy,Virgo,8.4
-NGC 2323  ,105.8,-8.333333333,Open Cluster,Monocerus,6.3
-NGC 5194 Whirlpool Galaxy,202.475,47.2,Spiral Galaxy,Canes Venatici,8.4
-NGC 7654  ,351.05,61.58333333,Open Cluster,Cassiopeia,7.3
-NGC 5024  ,198.225,18.16666667,Globular Cluster,Coma Berenices,7.6
-NGC 6715  ,283.775,-30.48333333,Globular Cluster,Sagittarius,7.6
-NGC 6809  ,295,-30.96666667,Globular Cluster,Sagittarius,6.3
-NGC 6779  ,289.15,30.18333333,Globular Cluster,Lyra,8.3
-NGC 6720 Ring Nebula,283.4,33.03333333,Planetary Nebula,Lyra,8.8
-NGC 4579  ,189.425,11.81666667,Spiral Galaxy,Virgo,9.7
-NGC 4621  ,190.5,11.65,Elliptical Galaxy,Virgo,9.6
-NGC 4649  ,190.925,11.55,Elliptical Galaxy,Virgo,8.8
-NGC 4303  ,185.475,4.466666667,Spiral Galaxy,Virgo,9.7
-NGC 6266  ,255.3,-30.11666667,Globular Cluster,Ophiucus,6.5
-NGC 5055 Sunflower Galaxy,198.95,42.03333333,Spiral Galaxy,Canes Venatici,8.6
-NGC 4826 Blackeye Galaxy,194.175,21.68333333,Spiral Galaxy,Coma Berenices,8.5
-NGC 3623  ,169.725,13.08333333,Spiral Galaxy,Leo,9.3
-NGC 3627  ,170.05,12.98333333,Spiral Galaxy,Leo,8.9
-NGC 2682  ,132.6,11.81666667,Open Cluster,Cancer,6.1
-NGC 4590  ,189.875,-26.75,Globular Cluster,Hydra,7.8
-NGC 6637  ,277.85,-32.35,Globular Cluster,Sagittarius,7.6
-NGC 6681  ,280.8,-32.3,Globular Cluster,Sagittarius,7.9
-NGC 6838  ,298.45,18.78333333,Globular Cluster,Sagitta,8.3
-NGC 6981,313.375,-12.53333333,Globular Cluster,Aquarius,9.3
-NGC 6994  Group of 4 stars,314.75,-12.63333333,Group/Asterism,Aquarius,9
-NGC 628 ,24.175,15.78333333,Spiral Galaxy,Pisces,9.4
-NGC 6864  ,301.525,-21.91666667,Globular Cluster,Sagittarius,8.5
-"NGC 650 Little Dumbell, Cork, Butterfly Nebula",25.575,51.56666667,Planetary Nebula,Perseus,10.1
-NGC 1068 Cetus A,40.675,0.016666667,Spiral Galaxy,Cetus,8.9
-NGC 2068  ,86.675,0.05,Diffuse Nebula,Orion,8.3
-NGC 1904  ,81.125,-24.55,Globular Cluster,Lepus,7.7
-NGC 6093  ,244.25,-22.98333333,Globular Cluster,Scorpius,7.3
-NGC 3031 Bode¹s Galaxy,148.9,69.06666667,Spiral Galaxy,Ursa Major,6.9
-NGC 3034 Cigar Galaxy,148.95,69.68333333,Irregular Galaxy,Ursa Major,8.4
-NGC 5236 Southern Pinwheel Galaxy,204.25,-29.86666667,Spiral Galaxy,Hydra,7.6
-NGC 4374  ,186.275,12.88333333,Lenticular (S0) Galaxy,Virgo,9.1
-NGC 4382  ,186.35,18.18333333,Lenticular (S0) Galaxy,Coma Berenices,9.1
-NGC 4406  ,186.55,12.95,Lenticular (S0) Galaxy,Virgo,8.9
-NGC 4486 Virgo A,187.7,12.4,Elliptical Galaxy,Virgo,8.6
-NGC 4501  ,188,14.41666667,Spiral Galaxy,Coma Berenices,9.6
-NGC 4552  ,188.925,12.55,Elliptical Galaxy,Virgo,9.8
-NGC 4569  ,189.2,13.16666667,Spiral Galaxy,Virgo,9.5
-NGC 4548  ,188.85,14.5,Spiral Galaxy,Coma Berenices,10.2
-NGC 6341  ,259.275,43.13333333,Globular Cluster,Hercules,6.4
-NGC 2447  ,116.15,-23.86666667,Open Cluster,Puppis,6
-NGC 4736  ,192.725,41.11666667,Spiral Galaxy,Canes Venatici,8.2
-NGC 3351  ,161,11.7,Spiral Galaxy,Leo,9.7
-NGC 3368  ,161.7,11.81666667,Spiral Galaxy,Leo,9.2
-NGC 3587 Owl Nebula,168.7,55.01666667,Planetary Nebula,Ursa Major,9.9
-NGC 4192  ,183.45,14.9,Spiral Galaxy,Coma Berenices,10.1
-NGC 4254  ,184.7,14.41666667,Spiral Galaxy,Coma Berenices,9.9
-NGC 4321  ,185.725,15.81666667,Spiral Galaxy,Coma Berenices,9.3
-NGC 5457 Pinwheel Galaxy,210.8,54.35,Spiral Galaxy,Ursa Major,7.9
-NGC 5866 Spindle Galaxy,226.625,55.76666667,Lenticular (S0) Galaxy,Draco,9.9
-NGC 581,23.3,60.7,Open Cluster,Cassiopeia,7.4
-NGC 4594 Sombrero Galaxy,190,-11.61666667,Spiral Galaxy,Virgo,8
-NGC 3379,161.95,12.58333333,Elliptical Galaxy,Leo,9.3
-NGC 4258,184.75,47.3,Spiral Galaxy,Canes Venatici,8.4
-NGC 6171,248.125,-13.05,Globular Cluster,Ophiucus,7.9
-NGC 3556,167.875,55.66666667,Spiral Galaxy,Ursa Major,10
-NGC 3992,179.4,53.38333333,Spiral Galaxy,Ursa Major,9.8
-NGC 205 Satellite of M31,10.1,41.68333333,Elliptical Galaxy,Andromeda,8.5
-Adhara,104.5,-28.96666667,Binary System,Canis Major,1.5
-Aldebaran,68.75,16.5,Red Giant,Taurus,0.86
-Altair,297.5,8.866666667,Main Sequence,Aquila,0.76
-Antares,247.25,-26.41666667,Red Supergiant,Scorpius,1.6
-Arcturus,213.75,19.16666667,Red Giant,Bootes,-0.05
-Bellatrix,81.25,6.333333333,Blue Giant,Orion,1.64
-Betelguese,88.75,7.4,Red Supergiant,Orion,0.5
-Capella,79,45.98333333,Four Star System,Auriga,0.08
-Castor,113.5,31.88333333,Six Star System,Gemini,1.93
-Deneb,310.25,45.26666667,Blue Giant,Cygnus,1.25
-Elnath,81.5,28.6,Binary System,Taurus,1.65
-Polaris,37.75,89.25,Triple Star System,Ursa Minor,1.9
-Pollux,116.25,28.01666667,Orange Giant,Gemini,1.14
-Procyon,114.75,5.216666667,Binary System,Canis Minor,0.34
-Regulus,152,11.96666667,Binary System,Leo,1.4
-Rigel,78.5,-8.2,Blue Supergiant,Orion,0.13
-Shaula,263.25,-37.1,Triple Star System,Scorpius,1.62
-Sirius,101.25,-16.7,Binary System,Canis Major,-1.46
-Spica,201.25,-11.15,Binary System,Virgo,0.97
-Vega,279,38.78333333,Variable Star,Lyra,0.026
+Name,RA,Dec,Type,Subtype,Constellation,V Mag
+NGC 1952 Crab Nebula,83.625,22.01666667,SupernovaRemnant,SupernovaRemnant,Taurus,8.4
+NGC 7089,323.375,-0.816666667,Cluster,Globular,Aquarius,6.5
+NGC 5272,205.55,28.38333333,Cluster,Globular,Canes Venatici,6.2
+NGC 6121,245.9,-26.53333333,Cluster,Globular,Scorpius,5.6
+NGC 5904,229.65,2.083333333,Cluster,Globular,Serpens Caput,5.6
+NGC 6405 Butterfly Cluster,265.025,-32.21666667,Cluster,Open,Scorpius,5.3
+NGC 6475 Ptolemy¹s Cluster,268.475,-34.81666667,Cluster,Open,Scorpius,4.1
+NGC 6523 Lagoon Nebula,270.95,-24.38333333,Nebula,Diffuse,Sagittarius,6
+NGC 6333,259.8,-18.51666667,Cluster,Globular,Ophiucus,7.7
+NGC 6254,254.275,-4.1,Cluster,Globular,Ophiucus,6.6
+NGC 6705 Wild Duck Cluster,282.775,-6.266666667,Cluster,Open,Scutum,6.3
+NGC 6218,251.8,-1.95,Cluster,Globular,Ophiucus,6.7
+NGC 6205 Hercules Globular Cluster,250.425,36.46666667,Cluster,Globular,Hercules,5.8
+NGC 6402,264.4,-3.25,Cluster,Globular,Ophiucus,7.6
+NGC 7078,322.5,12.16666667,Cluster,Globular,Pegasus,6.2
+NGC 6611 Eagle Nebula Cluster,274.7,-13.78333333,Cluster,Open,Serpens Claudia,6.4
+"NGC 6618 Omega, Swan, Horseshoe Nebula",275.2,-16.18333333,Nebula,Diffuse,Sagittarius,7
+NGC 6613,274.975,-17.13333333,Cluster,Open,Sagittarius,7.5
+NGC 6273,255.65,-26.26666667,Cluster,Globular,Ophiucus,6.8
+NGC 6514 Trifid Nebula,270.575,-23.03333333,Nebula,Diffuse,Sagittarius,9
+NGC 6531,271.15,-22.5,Cluster,Open,Sagittarius,6.5
+NGC 6656,279.1,-23.9,Cluster,Globular,Sagittarius,5.1
+NGC 6494,269.2,-19.01666667,Cluster,Open,Sagittarius,6.9
+NGC 6603 Milky Way Patch,274.6,-18.41666667,StarCloud,StarCloud,Sagittarius,4.6
+IC 4725,277.925,-19.23333333,Cluster,Open,Sagittarius,6.5
+NGC 6694,281.3,-9.4,Cluster,Open,Scutum,8
+NGC 6853 Dumbbell Nebula,299.9,22.71666667,Nebula,Planetary,Vulpecula,7.4
+NGC 6626,276.125,-24.86666667,Cluster,Globular,Sagittarius,6.8
+NGC 6913,305.975,38.53333333,Cluster,Open,Cygnus,7.1
+NGC 7099,325.1,-23.18333333,Cluster,Globular,Capricornus,7.2
+NGC 224 Andromeda Galaxy,10.675,41.26666667,Galaxy,Spiral,Andromeda,3.4
+NGC 221 Satellite of M31,10.675,40.86666667,Galaxy,Elliptical,Andromeda,8.1
+NGC 598 Triangulum-Pinwheel Galaxy,23.475,30.65,Galaxy,Spiral,Triangulum,5.7
+NGC 1039,40.5,42.78333333,Cluster,Open,Perseus,5.5
+NGC 2168,92.225,24.33333333,Cluster,Open,Gemini,5.3
+NGC 1960,84.025,34.13333333,Cluster,Open,Auriga,6.3
+NGC 2099,88.1,32.55,Cluster,Open,Auriga,6.2
+NGC 1912,82.175,35.83333333,Cluster,Open,Auriga,7.4
+NGC 7092,323.05,48.43333333,Cluster,Open,Cygnus,5.2
+Winecke 4,185.55,58.08333333,Star,Double,Ursa Major,9.3
+NGC 2287,101.75,-20.73333333,Cluster,Open,Canis Major,4.6
+NGC 1976 Great Orion Nebula,83.85,-5.45,Nebula,Diffuse,Orion,4
+NGC 1982 de Mairan¹s Nebula,83.9,-5.266666667,Nebula,Diffuse,Orion,9
+NGC 2632 Beehive Cluster (Praesepe),130.025,19.98333333,Cluster,Open,Cancer,3.7
+"Pleiades, Subaru, Seven Sisters",56.75,24.12,Cluster,Open,Taurus,1.6
+NGC 2437,115.45,-14.81666667,Cluster,Open,Puppis,6
+NGC 2422,114.15,-14.5,Cluster,Open,Puppis,5.2
+NGC 2548,123.45,-5.8,Cluster,Open,Hydra,5.5
+NGC 4472,187.45,8,Galaxy,Elliptical,Virgo,8.4
+NGC 2323,105.8,-8.333333333,Galaxy,Open,Monocerus,6.3
+NGC 5194 Whirlpool Galaxy,202.475,47.2,Galaxy,Spiral,Canes Venatici,8.4
+NGC 7654,351.05,61.58333333,Cluster,Open,Cassiopeia,7.3
+NGC 5024,198.225,18.16666667,Cluster,Globular,Coma Berenices,7.6
+NGC 6715,283.775,-30.48333333,Cluster,Globular,Sagittarius,7.6
+NGC 6809,295,-30.96666667,Cluster,Globular,Sagittarius,6.3
+NGC 6779,289.15,30.18333333,Cluster,Globular,Lyra,8.3
+NGC 6720 Ring Nebula,283.4,33.03333333,Nebula,Planetary,Lyra,8.8
+NGC 4579,189.425,11.81666667,Galaxy,Spiral,Virgo,9.7
+NGC 4621,190.5,11.65,Galaxy,Elliptical,Virgo,9.6
+NGC 4649,190.925,11.55,Galaxy,Elliptical,Virgo,8.8
+NGC 4303,185.475,4.466666667,Galaxy,Spiral,Virgo,9.7
+NGC 6266,255.3,-30.11666667,Cluster,Globular,Ophiucus,6.5
+NGC 5055 Sunflower Galaxy,198.95,42.03333333,Galaxy,Spiral,Canes Venatici,8.6
+NGC 4826 Blackeye Galaxy,194.175,21.68333333,Galaxy,Spiral,Coma Berenices,8.5
+NGC 3623,169.725,13.08333333,Galaxy,Spiral,Leo,9.3
+NGC 3627,170.05,12.98333333,Galaxy,Spiral,Leo,8.9
+NGC 2682,132.6,11.81666667,Cluster,Open,Cancer,6.1
+NGC 4590,189.875,-26.75,Cluster,Globular,Hydra,7.8
+NGC 6637,277.85,-32.35,Cluster,Globular,Sagittarius,7.6
+NGC 6681,280.8,-32.3,Cluster,Globular,Sagittarius,7.9
+NGC 6838,298.45,18.78333333,Cluster,Globular,Sagitta,8.3
+NGC 6981,313.375,-12.53333333,Cluster,Globular,Aquarius,9.3
+NGC 6994 Group of 4 stars,314.75,-12.63333333,Asterism,Asterism,Aquarius,9
+NGC 628,24.175,15.78333333,Galaxy,Spiral,Pisces,9.4
+NGC 6864  ,301.525,-21.91666667,Cluster,Globular,Sagittarius,8.5
+"NGC 650 Little Dumbell, Cork, Butterfly Nebula",25.575,51.56666667,Nebula,Planetary,Perseus,10.1
+NGC 1068 Cetus A,40.675,0.016666667,Galaxy,Spiral,Cetus,8.9
+NGC 2068,86.675,0.05,Nebula,Diffuse,Orion,8.3
+NGC 1904,81.125,-24.55,Cluster,Globular,Lepus,7.7
+NGC 6093,244.25,-22.98333333,Cluster,Globular,Scorpius,7.3
+NGC 3031 Bode¹s Galaxy,148.9,69.06666667,Galaxy,Spiral,Ursa Major,6.9
+NGC 3034 Cigar Galaxy,148.95,69.68333333,Galaxy,Irregular,Ursa Major,8.4
+NGC 5236 Southern Pinwheel Galaxy,204.25,-29.86666667,Galaxy,Spiral,Hydra,7.6
+NGC 4374,186.275,12.88333333,Galaxy,Lenticular,Virgo,9.1
+NGC 4382,186.35,18.18333333,Galaxy,Lenticular,Coma Berenices,9.1
+NGC 4406,186.55,12.95,Galaxy,Lenticular,Virgo,8.9
+NGC 4486 Virgo A,187.7,12.4,Galaxy,Elliptical,Virgo,8.6
+NGC 4501,188,14.41666667,Galaxy,Spiral,Coma Berenices,9.6
+NGC 4552,188.925,12.55,Galaxy,Elliptical,Virgo,9.8
+NGC 4569,189.2,13.16666667,Galaxy,Spiral,Virgo,9.5
+NGC 4548,188.85,14.5,Galaxy,Spiral,Coma Berenices,10.2
+NGC 6341,259.275,43.13333333,Cluster,Globular,Hercules,6.4
+NGC 2447,116.15,-23.86666667,Cluster,Open,Puppis,6
+NGC 4736,192.725,41.11666667,Galaxy,Spiral,Canes Venatici,8.2
+NGC 3351,161,11.7,Galaxy,Spiral,Leo,9.7
+NGC 3368,161.7,11.81666667,Galaxy,Spiral,Leo,9.2
+NGC 3587 Owl Nebula,168.7,55.01666667,Nebula,Planetary,Ursa Major,9.9
+NGC 4192,183.45,14.9,Galaxy,Spiral,Coma Berenices,10.1
+NGC 4254,184.7,14.41666667,Galaxy,Spiral,Coma Berenices,9.9
+NGC 4321,185.725,15.81666667,Galaxy,Spiral,Coma Berenices,9.3
+NGC 5457 Pinwheel Galaxy,210.8,54.35,Galaxy,Spiral,Ursa Major,7.9
+NGC 5866 Spindle Galaxy,226.625,55.76666667,Galaxy,Lenticular,Draco,9.9
+NGC 581,23.3,60.7,Cluster,Open,Cassiopeia,7.4
+NGC 4594 Sombrero Galaxy,190,-11.61666667,Galaxy,Spiral,Virgo,8
+NGC 3379,161.95,12.58333333,Galaxy,Elliptical,Leo,9.3
+NGC 4258,184.75,47.3,Galaxy,Spiral,Canes Venatici,8.4
+NGC 6171,248.125,-13.05,Cluster,Globular,Ophiucus,7.9
+NGC 3556,167.875,55.66666667,Galaxy,Spiral,Ursa Major,10
+NGC 3992,179.4,53.38333333,Galaxy,Spiral,Ursa Major,9.8
+NGC 205 Satellite of M31,10.1,41.68333333,Galaxy,Elliptical,Andromeda,8.5
+Adhara,104.5,-28.96666667,Star,Binary,Canis Major,1.5
+Aldebaran,68.75,16.5,Star,RedGiant,Taurus,0.86
+Altair,297.5,8.866666667,Star,MainSequence,Aquila,0.76
+Antares,247.25,-26.41666667,Star,RedSupergiant,Scorpius,1.6
+Arcturus,213.75,19.16666667,Star,RedGiant,Bootes,-0.05
+Bellatrix,81.25,6.333333333,Star,BlueGiant,Orion,1.64
+Betelguese,88.75,7.4,Star,RedSupergiant,Orion,0.5
+Capella,79,45.98333333,Star,FourStars,Auriga,0.08
+Castor,113.5,31.88333333,Star,SixStars,Gemini,1.93
+Deneb,310.25,45.26666667,Star,BlueGiant,Cygnus,1.25
+Elnath,81.5,28.6,Star,Binary,Taurus,1.65
+Polaris,37.75,89.25,Star,Triple,Ursa Minor,1.9
+Pollux,116.25,28.01666667,Star,OrangeGiant,Gemini,1.14
+Procyon,114.75,5.216666667,Star,Binary,Canis Minor,0.34
+Regulus,152,11.96666667,Star,Binary,Leo,1.4
+Rigel,78.5,-8.2,Star,BlueSupergiant,Orion,0.13
+Shaula,263.25,-37.1,Star,Triple,Scorpius,1.62
+Sirius,101.25,-16.7,Star,Binary,Canis Major,-1.46
+Spica,201.25,-11.15,Star,Binary,Virgo,0.97
+Vega,279,38.78333333,Star,Variable,Lyra,0.026
```

### Comparing `kirkwoodnight-0.9/kirkwoodnight/source.py` & `kirkwoodnight-1.0.0/kirkwoodnight/source.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# version 0.5
+# version 0.14
 
-# basic imports
+# basic importsl 
+import sys
 import os
 import numpy as np
 import pandas as pd
+import pkg_resources
 
 # date/time functionality
 import datetime
 from datetime import date
 
 # color and visualization
 from tabulate import tabulate
 from colorama import Fore
 
 # skyfield (for locations of solar system objects)
 import skyfield
-import skyfield
 from skyfield.api import load
 from skyfield.api import position_of_radec, load_constellation_map, load_constellation_names
 from skyfield.magnitudelib import planetary_magnitude
 
 # astropy (coordinates, units, date/time functionality)
 from astropy.coordinates import SkyCoord
 import astropy.units as u
@@ -32,20 +33,27 @@
 from astroplan import FixedTarget
 from astropy.table import QTable
 from astroplan.utils import time_grid_from_range
 from astroplan import Observer
 from astroplan import (AltitudeConstraint, AirmassConstraint,
                        AtNightConstraint, MoonIlluminationConstraint, MoonSeparationConstraint)
 
+# kirkwoodnight
+from kirkwoodnight import plotting
+
 def make_planet_table(date_str):
-    '''
+    '''Make Planet Table
+
     Generates AstroPy Table with positions (RA, Dec) of solar system planets on the given date.
     
-    Input: Desired date (str, formatted as "YYYY-MM-DD")
-    Output: Table of RA/dec for each object (AstroPy Table)
+    Args:
+        date_str (str): Desired date (str, formatted as "YYYY-MM-DD")
+
+    Returns:
+        df (DataFrame): Table of RA/dec for each object (AstroPy Table)
     '''
 
     y,m,d = [int(num) for num in date_str.split("-")] # split input date into constituents
 
     ts = load.timescale()
     t = ts.utc(y, m, d)
     planets = load('de421.bsp') # load ephemerides
@@ -53,14 +61,15 @@
     earth = planets["earth"] # establish earth location
     barycentric = earth.at(t)
 
     # other 7 planets
     pl_l = ["mercury", "venus", "mars", "jupiter barycenter", "saturn barycenter", "uranus barycenter", "neptune barycenter"]
     pl_names = ["Mercury", "Venus", "Mars", "Jupiter", "Saturn", "Uranus", "Neptune"]
     type_l = ["Planet"]*len(pl_names)
+    subtype_l = ["Terrestrial", "Terrestrial", "Terrestrial", "GasGiant", "GasGiant", "IceGiant", "IceGiant"]
     mag_l = []
     ra_l = []
     dec_l = []
 
     # grab position of every other planet
     for pl in pl_l:
         planet = planets[pl]
@@ -74,35 +83,32 @@
     constellation_at = load_constellation_map() 
     pos = position_of_radec(np.array(ra_l)/15, np.array(dec_l))
     const_abbrev = constellation_at(pos)
     const_name_dict = dict(load_constellation_names())
     const_l = [const_name_dict[abbrev] for abbrev in const_abbrev]
         
     # return pandas dataframe with info for planets
-    df = pd.DataFrame({"Name": pl_names, "RA": ra_l, "Dec": dec_l, "Type": type_l, "Constellation": const_l, "Magnitude": mag_l})
+    df = pd.DataFrame({"Name": pl_names, "RA": ra_l, "Dec": dec_l, "Type": type_l, "Subtype": subtype_l, "Constellation": const_l, "V Mag": mag_l})
     return df
 
 
 def make_constraints(alt_lim = (10, 80), moon_sep = 5, max_airmass = None, night_type = None, moon_illum = None):
-    '''
-    Creates list of desired observational constraints for use in sim_kirkwood_planets. Intended only as a helper function.
-    
-    Inputs (to be called in sim_kirkwood_obs, if needed)
-    -----------------------------
-    alt_lim (tuple): Lower and upper bounds (in deg) on allowable altitude of telescope, default is (10, 80)
-    moon_sep (float): Minimum angular separation (in deg) from moon, default is 5
-    max_airmass (float, optional): Maximum allowable airmass
-    night_type (str, optional): Defines beginning and end of night, options are "civil", "naut", and "astro"
-                        respectively for "civilian", "nautical", and "astronomical" definitions of twilight
-    moon_illum (str, optional): Allowable moon phase, options are "grey" and "dark"
+    '''Make Constraints
+
+    Creates list of desired observational constraints for use in sim_kirkwood_obs. Intended only as a helper function.
     
+    Args: (to be called in sim_kirkwood_obs, if needed)
+        alt_lim (tuple): Lower and upper bounds (in deg) on allowable altitude of telescope, default is (20, 80)
+        moon_sep (float): Minimum angular separation (in deg) from moon, default is 5
+        max_airmass (float, optional): Maximum allowable airmass
+        night_type (str, optional): Defines beginning and end of night, options are "civil", "naut", and "astro" respectively for "civilian", "nautical", and "astronomical" definitions of twilight
+        moon_illum (str, optional): Allowable moon phase, options are "grey" and "dark"
     
-    Output
-    ---------------------------
-    List of observational constraints (List of Astroplan objects)
+    Returns:
+        constraints (list): List of observational constraints (List of Astroplan objects)
     '''
     
     constraints = [AltitudeConstraint(alt_lim[0]*u.deg, alt_lim[1]*u.deg), MoonSeparationConstraint(moon_sep*u.deg)]
     if max_airmass:
         constraints.append(AirmassConstraint(max_airmass))
     if night_type == "civ":
         constraints.append(AtNightConstraint.twilight_civil())
@@ -114,39 +120,28 @@
         constraints.append(MoonIlluminationConstraint.grey())
     if night_type == "dark":
         constraints.append(MoonIlluminationConstraint.dark()) 
         
     return constraints
 
 def make_obs_grid(kirkwood, constraints, targets, t1_ust, t2_ust, dt = 0.5):
-    '''
+    '''Make Observation Grid
+
     Creates grids (NumPy arrays) defining observational efficacy for each object during the desired night.
     Intended only as a helper function for sim_kirkwood_obs.
     
-    Inputs
-    -----------------------------
-    kirkwood (Astroplan Observer object): Object defining location of Kirkwood observatory.
-                                            Passed automatically from sim_kirkwood_obs, does not require user alteration.
-    
-    constraints(list of Astroplan Constraint objects): Output from make_constraints. Passed automatically from
-                                                        sim_kirkwood_obs, does not require user alteration.
-    
-    targets (list of Astroplan Target objects): List of objects definiting positions of target objects.
-                                                Passed automatically from sim_kirkwood_obs, does not require user alteration.
-    
-    t1_ust, t2_ust (AstroPy.Time objects): Starting and ending time of observations in Universal Standard Time.
-                                            Passed autmoatically form sim_kirkwood_obs, does not require user alteration.
-    
-    dt (float): Time interval of output observing schedule (in hours), default is 0.5 (30 mins). 
-                Can be called directly in sim_kirkwood_obs, if needed.)
-    
-    Output
-    ------------------------------
-    time_grid (NumPy array): time array for observing schedule (in UST) expressed as Julian Date
+    Args:
+        kirkwood (Astroplan Observer object): Object defining location of Kirkwood observatory. Passed automatically from sim_kirkwood_obs, does not require user alteration.
+        constraints (list): Output from make_constraints (list of Astroplan Constraint objects). Passed automatically from sim_kirkwood_obs, does not require user alteration.
+        targets (list): List of objects definiting positions of target objects (Astroplan Target objects). Passed automatically from sim_kirkwood_obs, does not require user alteration.
+        t1_ust, t2_ust (AstroPy.Time objects): Starting and ending time of observations in Universal Standard Time. Passed autmoatically form sim_kirkwood_obs, does not require user alteration.
+        dt (float): Time interval of output observing schedule (in hours), default is 0.5 (30 mins). Can be called directly in sim_kirkwood_obs, if needed.)
     
+    Returns:
+        time_grid (array): time array for observing schedule (in UST) expressed as Julian Date
     
     '''
     
     dt *= u.hour # add astropy units to dt
     grid_list = []
     time_grid = time_grid_from_range([t1_ust, t2_ust], # create time grid
                                  time_resolution=dt)
@@ -168,41 +163,38 @@
     obs_percent = np.sum(total_obs, axis = 1)/total_obs.shape[1]
     print()
     return time_grid, total_obs, obs_percent
 
 
 def sim_kirkwood_obs(date = str(date.today()), start_time = str(datetime.datetime.now().time()), duration = 4,
                         alt_lim = (10, 80), moon_sep = 5, max_airmass = None, night_type = None, moon_illum = None, dt = 0.5):
-    '''
+    '''Simulate Kirkwood Observation
+
     Given date, time, and duration of an observing run (with optional observational constraints),
     prints table of object positions ranked by duration of observability, as well as rough observing schedule 
-    detailing blocks of time when each object will be observable during the run.
-
-    With user input of desired objects, saves text files with general info, sky positions, and observability for each object. 
-    
-    Required Inputs:
-    -----------------------------
-    date (str): desired date of observation, formatted as "YYYY-MM-DD", default is present day
-    start_time (str): desired start time of observing run (in local time zone), formatted as "HH:MM", defaults to current clock time
-    duration (float): approximate duration of observing run (in hours), defaults to 4
-    
-                
-    Optional (Keyword) Inputs:
-    -----------------------------
-    All constraint keyword arguments in make_constraints, as well as the dt argument for make_obs_grid.
-    
-    Output
-    ------------------------------
-    Prints table of objects, ranked by duration of observability, with positions in RA/dec and alt/az
-    Prints rough observing schedule detailing blocks of observing run when each object is observable
-    (i.e. satisfies all imposed observational constraints)
+    detailing blocks of time when each object will be observable during the run. With user input of desired
+    objects, saves text files with general info, sky positions, and observability for each object. 
     
+    Args:
+        date (str): desired date of observation, formatted as "YYYY-MM-DD", default is present day
+        start_time (str): desired start time of observing run (in local time zone), formatted as "HH:MM", defaults to current clock time
+        duration (float): approximate duration of observing run (in hours), defaults to 4
+        alt_lim (tuple, optional): arg of make_constraints
+        moon_sep (float, optional): arg of make_constraints
+        max_airmass (float, optional): arg of make_constraints
+        night_type (str, optional): arg of make_constraints
+        moon_illum (str, optional): arg of make_constraints
+        dt (float, optional): time interval for observing grid, argument for make_obs_grid
+    
+    Returns:
+        target_df (DataFrame): pandas DataFrame containing the target info for those selected for observation.
+        time_df (DataFrame): pandas DataFrame containing the target observing plans as a function of time.
     
     '''
-    #print(date, start_time)
+
     t1 = Time(date + " " + start_time) # convert start time to time object
     t2 = t1 + TimeDelta(duration*u.h) # make end time and add units
     
     # define Observer object, input location of Kirkwood
     kirkwood = Observer(longitude=-86.5264*u.deg, latitude=39.1653*u.deg,
                   elevation=235*u.m, name="Kirkwood", timezone="US/East-Indiana")
     
@@ -210,15 +202,16 @@
     t1_ust, t2_ust = t1 + TimeDelta(4*u.h), t2 + TimeDelta(4*u.h)
     time_range = Time([t1_ust, t2_ust])
 
     # make table of planets
     planet_df = make_planet_table(date)
     
     # make table of deep sky objects
-    deep_sky_df = pd.read_csv("obj_list.csv")
+    stream = pkg_resources.resource_stream(__name__, 'data/obj_list.csv')
+    deep_sky_df = pd.read_csv(stream, encoding = "latin-1")
     target_df = pd.concat([planet_df, deep_sky_df])
 
     # make astropy table to feed into astroplan
     target_table_pd = target_df[["Name", "RA", "Dec"]]
     target_table = Table.from_pandas(target_table_pd)
     targets = [FixedTarget(coord=SkyCoord(ra=ra*u.deg, dec=dec*u.deg), name=name) for name, ra, dec in target_table]
     
@@ -226,117 +219,165 @@
     constraints = make_constraints(alt_lim, moon_sep, max_airmass, night_type, moon_illum)
     # make time grid and raw observing tables/schedule
     time_grid, total_obs, obs_percent = make_obs_grid(kirkwood, constraints, targets, t1_ust, t2_ust, dt)
     
     # build dataframe of all targets, add column for observability fraction
     target_df["Obs. Frac."] = obs_percent
     target_df = target_df.set_index("Name")
-    target_df["Magnitude"] = target_df["Magnitude"].astype(float)
-    target_names_ordered = list(target_df.index) # save ordered list of target names, this is needed for later bookkeeping
-    target_df = target_df.sort_values(by=['Obs. Frac.', "Magnitude"], ascending = [False, True]) # sort table by observability and brightness
-    target_df = target_df.round(2) 
-
-    # user input for how many objects to display in printed tables
-    display_N = 20
-    print("How many objects would you like displayed? (Sorted by most observable, hit ENTER for default of 20, maximum is 130.)")
+    target_df["V Mag"] = target_df["V Mag"].astype(float)
+    target_names_all = list(target_df.index)
+    target_df = target_df.sort_values(by=['Obs. Frac.', "V Mag"], ascending = [False, True]) # sort table by observability and brightness
+    target_df = target_df.round(2)
+    target_df.insert(0, "ID", range(1, len(target_df) + 1))
+
+    types = list(set(target_df["Type"]))
+    types = [" " + item for item in types]
+    print("Is/are there a particular type(s) of object you would like to look at? The options are:\n")
+    print(",".join([i for i in types]))
+    print("\nPlease enter the type(s) of the objects you would like to observe, separated by commas (if multiple). Hit ENTER to observe all listed types.")
     var = input()
-    if var != "":
-        display_N  = int(var)
+    if var == "exit":
+            sys.exit()
+    if var!= "":
+        var = var.split(",")
+        target_df = target_df[target_df["Type"].isin(var)]
+        subtypes = list(set(target_df["Subtype"]))
+        subtypes = [" " + item for item in subtypes]
+        print("Is there a specific subtype of object you would like to look at? The options are:\n")
+        print(",".join([i for i in subtypes]))
+        print("\nPlease enter the subtype(s) of object you would like to observe, separated by commas (if multiple). Hit ENTER to observe all listed subtypes.")
+        subvar = input()
+        if subvar == "exit":
+            sys.exit()
+        if subvar != "":
+            subvar = subvar.split(",")
+            target_df = target_df[target_df["Subtype"].isin(subvar)]
+
+    display_N = len(target_df.index)
+
+    if display_N >= 20:
+        # user input for how many objects to display in printed tables
+        display_N = 20
+        print("How many objects would you like displayed? (Sorted by most observable, hit ENTER for default of 20. Maximum is %d)"%(len(target_df.index)))
+        var = input()
+        if var == "exit":
+            sys.exit()
+        if var != "":
+            display_N  = int(var)
+
+    target_df = target_df[:display_N]
+    target_names_ordered = list(target_df.index)
+    ids_ordered = list(target_df['ID'])
     
     # convert time array back to EST
     time_est = [t.datetime - datetime.timedelta(hours=4) for t in time_grid]
     time_labels = [t.strftime("%H:%M") for t in time_est]
     
     # make dataframe for observing schedule
     time_df = pd.DataFrame(total_obs, columns = time_labels)
-    time_df = time_df.replace([0, 1], [Fore.RED + "no"  + Fore.RESET, Fore.GREEN + 'YES' + Fore.RESET]) # add color
-    time_df.insert(0, "Name", target_names_ordered)
+    time_df.insert(0, "Name", target_names_all)
     time_df = time_df.set_index("Name")
-    time_df = time_df.reindex(target_df.index) # sort objects to be in same order as other table
-    
-    # add ID numbers to objects
-    target_df.insert(0, "ID", range(1, len(target_df) + 1))
-    time_df.insert(0, "ID", range(1, len(time_df) + 1))
+    time_df = time_df[time_df.index.isin(target_names_ordered)]
+    time_df = time_df.reindex(target_names_ordered) # sort objects to be in same order as other table
+    time_df = time_df.replace([0, 1], [Fore.RED + "no"  + Fore.RESET, Fore.GREEN + 'YES' + Fore.RESET]) # add color
+    time_df.insert(0, "ID", ids_ordered)
 
     # display information table
     print(tabulate(target_df[:display_N], headers = 'keys', tablefmt = 'psql'))
 
     # display schedule
     print(tabulate(time_df[:display_N], headers = 'keys', tablefmt = 'psql'))
 
-
     # user input for which object IDs they want to observe
-    print("Please enter the IDs of the objects you would like to observe, separated by commas. Hit ENTER to observe all listed objects.")
-
-    ids = input()
-
-    print("Generating files...")
-
-    if ids == "":
-        ids = list(range(1, display_N + 1))
-    else:
-        ids = ids.split(","); ids = [int(i) for i in ids]
-    
-    # limit info and schedule dataframes only to selected objects
-    selected_target_df = target_df.loc[target_df['ID'].isin(ids)]
-    selected_names = list(selected_target_df.index) # names of selected objects
-    selected_time_df = time_df.loc[time_df['ID'].isin(ids)]
-    selected_time_df = selected_time_df.replace([Fore.RED + "no"  + Fore.RESET, Fore.GREEN + 'YES' + Fore.RESET], ["no", "YES"])
-    
-    # remake astroplan targets for selected objects
-    selected_target_df_pos = selected_target_df[["RA", "Dec"]]
-    selected_target_df_pos.reset_index(inplace=True)
-    selected_target_table = Table.from_pandas(selected_target_df_pos)
-    selected_targets = [FixedTarget(coord=SkyCoord(ra=ra*u.deg, dec=dec*u.deg), name=name) for name, ra, dec in selected_target_table]
-
-    # create directories for output files
-    dir = "output"
-    os.makedirs(dir, exist_ok=True)
-    subdir = dir + "/" + str(datetime.datetime.now()).split(" ")[0] + "_" + str(datetime.datetime.now()).split(" ")[1][:8].replace(":", ".")
-    os.makedirs(subdir, exist_ok = True)
+    print("\nWould you like to generate infromation/schedule files for select objects? Type 'yes' or press ENTER to exit the program):")
+    var = input()
+    if var == "" or var == "exit":
+        sys.exit()
+    if var == "yes":
+        print("Please enter the IDs of the objects you would like to observe, separated by commas. Hit ENTER to observe all listed objects.")
+
+        ids = input()
+        if ids == "exit":
+            sys.exit()
+
+        print("Generating files...")
+
+        if ids == "":
+            ids = list(range(1, display_N + 1))
+        else:
+            ids = ids.split(","); ids = [int(i) for i in ids]
+    
+        # limit info and schedule dataframes only to selected objects
+        selected_target_df = target_df.loc[target_df['ID'].isin(ids)]
+        selected_names = list(selected_target_df.index) # names of selected objects
+        selected_time_df = time_df.loc[time_df['ID'].isin(ids)]
+        selected_time_df = selected_time_df.replace([Fore.RED + "no"  + Fore.RESET, Fore.GREEN + 'YES' + Fore.RESET], ["no", "YES"])
+    
+        # remake astroplan targets for selected objects
+        selected_target_df_pos = selected_target_df[["RA", "Dec"]]
+        selected_target_df_pos.reset_index(inplace=True)
+        selected_target_table = Table.from_pandas(selected_target_df_pos)
+        selected_targets = [FixedTarget(coord=SkyCoord(ra=ra*u.deg, dec=dec*u.deg), name=name) for name, ra, dec in selected_target_table]
+
+        # create directories for output files
+        dir = "output"
+        os.makedirs(dir, exist_ok=True)
+        subdir = dir + "/" + str(datetime.datetime.now()).split(" ")[0] + "_" + str(datetime.datetime.now()).split(" ")[1][:8].replace(":", ".")
+        os.makedirs(subdir, exist_ok = True)
 
     # loop over targets and calcluate alt and az for each time interval during the night
-    for i in range(len(selected_targets)):
-        alt, az = [], []
-        for t in time_grid:
-            t = Time(t.datetime)
-            alt.append(kirkwood.altaz(t, selected_targets[i]).alt.value)
-            az.append(kirkwood.altaz(t, selected_targets[i]).az.value)
-        obj = selected_names[i]
-        target_info = selected_target_df.loc[obj]
-        target_time = selected_time_df.loc[obj]
-        target_info = target_info.drop(labels=["ID"]) # final info for selected object
-        target_time = target_time.drop(labels=["ID"])
-        target_obs = list(target_time)
-        target_time = pd.DataFrame([time_labels, target_obs, alt, az])
-        target_time = target_time.T
-        target_time.columns = ["Time", "Observable", "Alt", 'Az']
-        target_time = target_time.set_index("Time") # final schedule (and alt/az) for selected object
+        for i in range(len(selected_targets)):
+            alt, az = [], []
+            for t in time_grid:
+                t = Time(t.datetime)
+                alt.append(kirkwood.altaz(t, selected_targets[i]).alt.value)
+                az.append(kirkwood.altaz(t, selected_targets[i]).az.value)
+            obj = selected_names[i]
+            target_info = selected_target_df.loc[obj]
+            target_time = selected_time_df.loc[obj]
+            #target_info = target_info.drop(labels=["ID"]) # final info for selected object
+            target_time = target_time.drop(labels=["ID"])
+            target_obs = list(target_time)
+            target_time = pd.DataFrame([time_labels, target_obs, alt, az])
+            target_time = target_time.T
+            target_time.columns = ["Time", "Observable", "Alt", 'Az']
+            target_time = target_time.set_index("Time") # final schedule (and alt/az) for selected object
 
-        # write info/schedule files for each object and save
-        filename = obj+"_summary.txt"
+            # write info/schedule files for each object and save
+            filename = obj+"_summary.txt"
                     
-        with open(subdir + "/" + filename, 'w') as f:
-            f.write(target_info.to_string() + "\n" + "\n")
-            f.write(target_time.to_string())
-    print("Info and schedule for selected objects saved as text files in " + subdir)
+            with open(subdir + "/" + filename, 'w') as f:
+                f.write(target_info.to_string() + "\n" + "\n")
+                f.write(target_time.to_string())
+                print("Info and schedule for selected objects saved as text files in " + subdir)
+    # plotting
+        print("\nWould you like to create sky charts for your observing run? Type 'yes' or press ENTER to exit the program:")
+        var = input()
+        if var == "":
+            sys.exit()
+        if var == "yes":
+            plotting.plot_it(subdir)
 
     # write and save log file
-    with open(subdir + "/" + "log", 'w') as f:
-        f.write("Date/Time:" + " " + str(datetime.datetime.now()) + "\n" + "\n")
-
-        f.write("Desired Date: " + str(date) + "\n")
-        f.write("Desired Start Time: " + str(start_time) + "\n")
-        f.write("Duration (hrs): " + str(duration) + "\n")
-        f.write("Altitude Range (deg): " + str(alt_lim[0]) + " to " + str(alt_lim[1]) + "\n")
-        f.write("Minimum Moon Separation (deg): " + str(moon_sep) + "\n")
-        f.write("Maximum Airmass: " + str(max_airmass) + "\n")
-        f.write("Twilight Convention: " + str(night_type) + "\n")
-        f.write("Lunar Illumination: " + str(moon_illum) + "\n")
-        f.write("Time Partition (hrs): " + str(dt) + "\n" + "\n")
-        f.write(str(len(selected_targets)) + " objects selected for observation: \n")
-        for obj in selected_names:
-            f.write(obj + "\n")
+        print("\nWould you like to save a log file? Type 'yes' or press ENTER to exit the program:")
+        var = input()
+        if var == "":
+            sys.exit()
+        if var == "yes":
+            with open(subdir + "/" + "log", 'w') as f:
+                f.write("Date/Time:" + " " + str(datetime.datetime.now()) + "\n" + "\n")
+                f.write("Desired Date: " + str(date) + "\n")
+                f.write("Desired Start Time: " + str(start_time) + "\n")
+                f.write("Duration (hrs): " + str(duration) + "\n")
+                f.write("Altitude Range (deg): " + str(alt_lim[0]) + " to " + str(alt_lim[1]) + "\n")
+                f.write("Minimum Moon Separation (deg): " + str(moon_sep) + "\n")
+                f.write("Maximum Airmass: " + str(max_airmass) + "\n")
+                f.write("Twilight Convention: " + str(night_type) + "\n")
+                f.write("Lunar Illumination: " + str(moon_illum) + "\n")
+                f.write("Time Partition (hrs): " + str(dt) + "\n" + "\n")
+                f.write(str(len(selected_targets)) + " objects selected for observation: \n")
+                for obj in selected_names:
+                    f.write(obj + "\n")
 
-    print("Log file saved in " + subdir)
+                print("Log file saved in " + subdir)
 
     return target_df, time_df
```

### Comparing `kirkwoodnight-0.9/setup.py` & `kirkwoodnight-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     reqs = []
     for line in open("requirements.txt", "r").readlines():
         reqs.append(line)
     return reqs
 
 setup(
     name="kirkwoodnight",
-    version="0.9",
+    version="1.0.0",
     packages=find_packages(),
 
     # Metadata
     author="Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang",
     author_email="armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu",
     description="Interactive command line tool to assist with observations at Kirkwood Observatory.",
     long_description=open('README.md').read(),
@@ -27,11 +27,11 @@
     entry_points={
         'console_scripts': [
             'kirkwoodnight = kirkwoodnight.command_line:main',
         ],
     },
 
     # Include additional files into the package
-    package_data={'': ['obj_list.csv']},
+    package_data={'': ['data/*.csv']},
 
     install_requires= get_requires(),
 )
```

