# Comparing `tmp/imephu-0.3.0.tar.gz` & `tmp/imephu-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imephu-0.3.0.tar", max compression
+gzip compressed data, was "imephu-0.4.0.tar", max compression
```

## Comparing `imephu-0.3.0.tar` & `imephu-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1102 2023-07-10 14:47:42.674953 imephu-0.3.0/LICENSE
--rw-r--r--   0        0        0     1015 2023-07-10 14:47:42.675169 imephu-0.3.0/README.md
--rw-r--r--   0        0        0      991 2023-07-12 17:32:34.545589 imephu-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      235 2023-07-12 17:32:34.546165 imephu-0.3.0/src/imephu/__init__.py
--rw-r--r--   0        0        0     1550 2023-07-10 14:47:42.735797 imephu-0.3.0/src/imephu/annotation/__init__.py
--rw-r--r--   0        0        0      746 2023-07-10 14:47:42.736360 imephu-0.3.0/src/imephu/annotation/general/__init__.py
--rw-r--r--   0        0        0     4480 2023-07-10 14:47:42.736748 imephu-0.3.0/src/imephu/annotation/general/arrow.py
--rw-r--r--   0        0        0     3879 2023-07-10 14:47:42.737079 imephu-0.3.0/src/imephu/annotation/general/circle.py
--rw-r--r--   0        0        0     2581 2023-07-10 14:47:42.737385 imephu-0.3.0/src/imephu/annotation/general/crosshairs.py
--rw-r--r--   0        0        0     1646 2023-07-10 14:47:42.737673 imephu-0.3.0/src/imephu/annotation/general/empty.py
--rw-r--r--   0        0        0     3021 2023-07-10 14:47:42.738079 imephu-0.3.0/src/imephu/annotation/general/group.py
--rw-r--r--   0        0        0     4428 2023-07-10 14:47:42.738417 imephu-0.3.0/src/imephu/annotation/general/line_path.py
--rw-r--r--   0        0        0     4425 2023-07-10 14:47:42.738680 imephu-0.3.0/src/imephu/annotation/general/rectangle.py
--rw-r--r--   0        0        0     5316 2023-07-10 14:47:42.738939 imephu-0.3.0/src/imephu/annotation/general/text.py
--rw-r--r--   0        0        0     9170 2023-07-10 14:47:42.739226 imephu-0.3.0/src/imephu/annotation/motion.py
--rw-r--r--   0        0        0    12102 2023-07-12 17:32:34.547123 imephu-0.3.0/src/imephu/cli.py
--rw-r--r--   0        0        0    12907 2023-07-10 14:47:42.739791 imephu-0.3.0/src/imephu/finder_chart.py
--rw-r--r--   0        0        0     9710 2023-07-10 14:47:42.740083 imephu-0.3.0/src/imephu/geometry.py
--rw-r--r--   0        0        0        0 2023-07-10 14:47:42.740215 imephu-0.3.0/src/imephu/py.typed
--rw-r--r--   0        0        0        0 2023-07-10 14:47:42.740669 imephu-0.3.0/src/imephu/salt/annotation/__init__.py
--rw-r--r--   0        0        0    12623 2023-07-12 17:32:34.547738 imephu-0.3.0/src/imephu/salt/annotation/nir.py
--rw-r--r--   0        0        0     3859 2023-07-10 14:47:42.741179 imephu-0.3.0/src/imephu/salt/annotation/rss.py
--rw-r--r--   0        0        0     1195 2023-07-10 14:47:42.741408 imephu-0.3.0/src/imephu/salt/annotation/salticam.py
--rw-r--r--   0        0        0     9004 2023-07-10 14:47:42.741632 imephu-0.3.0/src/imephu/salt/annotation/telescope.py
--rw-r--r--   0        0        0    15176 2023-07-12 17:32:34.548326 imephu-0.3.0/src/imephu/salt/finder_chart.py
--rw-r--r--   0        0        0     4859 2023-07-10 14:47:42.742110 imephu-0.3.0/src/imephu/salt/utils.py
--rw-r--r--   0        0        0    10440 2023-07-12 17:32:34.548999 imephu-0.3.0/src/imephu/schema.json
--rw-r--r--   0        0        0     9472 2023-07-10 14:47:42.742725 imephu-0.3.0/src/imephu/service/horizons.py
--rw-r--r--   0        0        0    15225 2023-07-10 14:47:42.742998 imephu-0.3.0/src/imephu/service/survey.py
--rw-r--r--   0        0        0     3680 2023-07-10 14:47:42.743218 imephu-0.3.0/src/imephu/utils.py
--rw-r--r--   0        0        0     1876 1970-01-01 00:00:00.000000 imephu-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-07-10 14:47:42.674953 imephu-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1015 2023-07-10 14:47:42.675169 imephu-0.4.0/README.md
+-rw-r--r--   0        0        0      991 2023-07-14 17:06:28.688837 imephu-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      235 2023-07-12 17:32:34.546165 imephu-0.4.0/src/imephu/__init__.py
+-rw-r--r--   0        0        0     1550 2023-07-10 14:47:42.735797 imephu-0.4.0/src/imephu/annotation/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-10 14:47:42.736360 imephu-0.4.0/src/imephu/annotation/general/__init__.py
+-rw-r--r--   0        0        0     4480 2023-07-10 14:47:42.736748 imephu-0.4.0/src/imephu/annotation/general/arrow.py
+-rw-r--r--   0        0        0     3879 2023-07-10 14:47:42.737079 imephu-0.4.0/src/imephu/annotation/general/circle.py
+-rw-r--r--   0        0        0     2581 2023-07-10 14:47:42.737385 imephu-0.4.0/src/imephu/annotation/general/crosshairs.py
+-rw-r--r--   0        0        0     1646 2023-07-10 14:47:42.737673 imephu-0.4.0/src/imephu/annotation/general/empty.py
+-rw-r--r--   0        0        0     3021 2023-07-10 14:47:42.738079 imephu-0.4.0/src/imephu/annotation/general/group.py
+-rw-r--r--   0        0        0     4428 2023-07-10 14:47:42.738417 imephu-0.4.0/src/imephu/annotation/general/line_path.py
+-rw-r--r--   0        0        0     4425 2023-07-10 14:47:42.738680 imephu-0.4.0/src/imephu/annotation/general/rectangle.py
+-rw-r--r--   0        0        0     5316 2023-07-10 14:47:42.738939 imephu-0.4.0/src/imephu/annotation/general/text.py
+-rw-r--r--   0        0        0     9170 2023-07-10 14:47:42.739226 imephu-0.4.0/src/imephu/annotation/motion.py
+-rw-r--r--   0        0        0    12400 2023-07-14 17:06:28.689624 imephu-0.4.0/src/imephu/cli.py
+-rw-r--r--   0        0        0    12907 2023-07-10 14:47:42.739791 imephu-0.4.0/src/imephu/finder_chart.py
+-rw-r--r--   0        0        0     9710 2023-07-10 14:47:42.740083 imephu-0.4.0/src/imephu/geometry.py
+-rw-r--r--   0        0        0        0 2023-07-10 14:47:42.740215 imephu-0.4.0/src/imephu/py.typed
+-rw-r--r--   0        0        0        0 2023-07-10 14:47:42.740669 imephu-0.4.0/src/imephu/salt/annotation/__init__.py
+-rw-r--r--   0        0        0    12623 2023-07-12 17:32:34.547738 imephu-0.4.0/src/imephu/salt/annotation/nir.py
+-rw-r--r--   0        0        0     4365 2023-07-14 17:06:28.691527 imephu-0.4.0/src/imephu/salt/annotation/rss.py
+-rw-r--r--   0        0        0     1195 2023-07-10 14:47:42.741408 imephu-0.4.0/src/imephu/salt/annotation/salticam.py
+-rw-r--r--   0        0        0     9004 2023-07-10 14:47:42.741632 imephu-0.4.0/src/imephu/salt/annotation/telescope.py
+-rw-r--r--   0        0        0    15615 2023-07-14 17:06:28.692233 imephu-0.4.0/src/imephu/salt/finder_chart.py
+-rw-r--r--   0        0        0     4859 2023-07-10 14:47:42.742110 imephu-0.4.0/src/imephu/salt/utils.py
+-rw-r--r--   0        0        0    10500 2023-07-14 17:06:28.692870 imephu-0.4.0/src/imephu/schema.json
+-rw-r--r--   0        0        0     9472 2023-07-10 14:47:42.742725 imephu-0.4.0/src/imephu/service/horizons.py
+-rw-r--r--   0        0        0    15225 2023-07-10 14:47:42.742998 imephu-0.4.0/src/imephu/service/survey.py
+-rw-r--r--   0        0        0     3680 2023-07-10 14:47:42.743218 imephu-0.4.0/src/imephu/utils.py
+-rw-r--r--   0        0        0     1876 1970-01-01 00:00:00.000000 imephu-0.4.0/PKG-INFO
```

### Comparing `imephu-0.3.0/LICENSE` & `imephu-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/README.md` & `imephu-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/pyproject.toml` & `imephu-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imephu"
-version = "0.3.0"
+version = "0.4.0"
 description = "Generate finder charts for astronomical observations."
 authors = ["Southern African Large Telescope"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `imephu-0.3.0/src/imephu/annotation/__init__.py` & `imephu-0.4.0/src/imephu/annotation/__init__.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/annotation/general/__init__.py` & `imephu-0.4.0/src/imephu/annotation/general/__init__.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/annotation/general/arrow.py` & `imephu-0.4.0/src/imephu/annotation/general/arrow.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/annotation/general/circle.py` & `imephu-0.4.0/src/imephu/annotation/general/circle.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/annotation/general/crosshairs.py` & `imephu-0.4.0/src/imephu/annotation/general/crosshairs.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/annotation/general/empty.py` & `imephu-0.4.0/src/imephu/annotation/general/empty.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/annotation/general/group.py` & `imephu-0.4.0/src/imephu/annotation/general/group.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/annotation/general/line_path.py` & `imephu-0.4.0/src/imephu/annotation/general/line_path.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/annotation/general/rectangle.py` & `imephu-0.4.0/src/imephu/annotation/general/rectangle.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/annotation/general/text.py` & `imephu-0.4.0/src/imephu/annotation/general/text.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/annotation/motion.py` & `imephu-0.4.0/src/imephu/annotation/motion.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/cli.py` & `imephu-0.4.0/src/imephu/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,16 +292,26 @@
         is_slot_mode = rss.get("slot-mode", False)
         return sfc.rss_imaging_finder_chart(
             fits=fits, general=general, is_slot_mode=is_slot_mode
         )
     elif instrument_mode == "spectroscopy":
         slit_width = Angle(rss["slit-width"])
         slit_height = Angle(rss["slit-height"])
+        if "reference-star" in rss:
+            reference_star = SkyCoord(
+                ra=rss["reference-star"]["ra"], dec=rss["reference-star"]["dec"]
+            )
+        else:
+            reference_star = None
         return sfc.rss_longslit_finder_chart(
-            fits=fits, general=general, slit_width=slit_width, slit_height=slit_height
+            fits=fits,
+            general=general,
+            slit_width=slit_width,
+            slit_height=slit_height,
+            reference_star=reference_star,
         )
     elif instrument_mode == "mos":
         mos_mask = MosMask.from_file(rss["file"])
         reference_star_box_width = (
             Angle(rss["reference-star-box-width"])
             if "reference-star-box-width" in rss
             else Angle(5 * u.arcsec)
```

### Comparing `imephu-0.3.0/src/imephu/finder_chart.py` & `imephu-0.4.0/src/imephu/finder_chart.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/geometry.py` & `imephu-0.4.0/src/imephu/geometry.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/salt/annotation/nir.py` & `imephu-0.4.0/src/imephu/salt/annotation/nir.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/salt/annotation/rss.py` & `imephu-0.4.0/src/imephu/salt/annotation/rss.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,14 +72,33 @@
         The annotation showing the longslit.
     """
     return RectangleAnnotation(
         fits_center, slit_width, slit_height, wcs=wcs, edgecolor="red", alpha=0.5
     ).rotate(fits_center, position_angle)
 
 
+def reference_star_annotation(reference_star: SkyCoord, wcs: WCS) -> CircleAnnotation:
+    """Return a circle highlighting a reference star.
+
+    Parameters
+    ----------
+    reference_star: `~astropy.coordinates.SkyCoord`
+        The central position of the finder chart, in right ascension and declination
+    wcs: `~astropy.wcs.WCS`
+        WCS object.
+    """
+    return CircleAnnotation(
+        reference_star,
+        10 * u.arcsec,
+        wcs,
+        edgecolor="red",
+        alpha=0.5,
+    )
+
+
 def mos_mask_annotation(
     mos_mask: MosMask, wcs: WCS, reference_star_box_width: Angle = 5 * u.arcsec
 ) -> GroupAnnotation:
     """Return the annotation for a MOS mask.
 
     The slits and boxes around the reference stars are included in the annotation.
```

### Comparing `imephu-0.3.0/src/imephu/salt/annotation/salticam.py` & `imephu-0.4.0/src/imephu/salt/annotation/salticam.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/salt/annotation/telescope.py` & `imephu-0.4.0/src/imephu/salt/annotation/telescope.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/salt/finder_chart.py` & `imephu-0.4.0/src/imephu/salt/finder_chart.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,38 +132,42 @@
 
 
 def rss_longslit_finder_chart(
     fits: Union[str, BinaryIO, os.PathLike[Any]],
     general: GeneralProperties,
     slit_width: Angle,
     slit_height: Angle,
+    reference_star: Optional[SkyCoord],
 ) -> FinderChart:
     """Return the finder chart for an RSS longslit observation.
 
     Parameters
     ----------
     fits: `str`, `path-like` or `binary file-like`
         FITS file to display.
     general: `GeneralProperties`
         Properties which are not specific to the instrument.
     slit_width: `~astropy.coordinates.Angle`
         The slit width, as an angle on the sky.
     slit_height: `~astropy.coordinates.Angle`
         The slit height, as an angle on the sky.
+    reference_star: `~astropy.coordinates.SkyCoord`, optional
+        The position of a reference star, in right ascension and declination.
 
     Returns
     -------
     `~imephu.finder_chart.FinderChart`
         The finder chart for an RSS longslit observation.
     """
     finder_chart = FinderChart(fits)
     annotation = _rss_longslit_observation_annotation(
         general=general,
         slit_width=slit_width,
         slit_height=slit_height,
+        reference_star=reference_star,
         wcs=finder_chart.wcs,
     )
     finder_chart.add_annotation(annotation)
     return finder_chart
 
 
 DEFAULT_REF_STAR_BOX_SIZE = Angle(5 * u.arcsec)
@@ -359,25 +363,32 @@
 def _rss_imaging_observation_annotation(
     general: GeneralProperties, is_slot_mode: bool, wcs: WCS
 ) -> GroupAnnotation:
     return _imaging_annotation(general, is_slot_mode, wcs)
 
 
 def _rss_longslit_observation_annotation(
-    general: GeneralProperties, slit_width: Angle, slit_height: Angle, wcs: WCS
+    general: GeneralProperties,
+    slit_width: Angle,
+    slit_height: Angle,
+    reference_star: SkyCoord,
+    wcs: WCS,
 ) -> GroupAnnotation:
     observation_annotation = _base_annotations(general, wcs)
     longslit_annotation = rss.longslit_annotation(
         fits_center=general.target.position,
         slit_width=slit_width,
         slit_height=slit_height,
         position_angle=general.position_angle,
         wcs=wcs,
     )
     observation_annotation.add_item(longslit_annotation)
+    if reference_star:
+        reference_star_annotation = rss.reference_star_annotation(reference_star, wcs)
+        observation_annotation.add_item(reference_star_annotation)
     return observation_annotation
 
 
 def _rss_mos_observation_annotation(
     general: GeneralProperties,
     mos_mask: MosMask,
     reference_star_box_width: Angle,
```

### Comparing `imephu-0.3.0/src/imephu/salt/utils.py` & `imephu-0.4.0/src/imephu/salt/utils.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/schema.json` & `imephu-0.4.0/src/imephu/schema.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9900841346153846%*

 * *Differences: {"'$defs'": "{'nir': {'properties': {'reference-star': {replace: OrderedDict([('$ref', "*

 * *            "'#/$defs/reference-star')])}}}, 'rss-spectroscopy': {'properties': {'reference-star': "*

 * *            "OrderedDict([('$ref', '#/$defs/reference-star')])}}, 'reference-star': "*

 * *            "OrderedDict([('type', 'object'), ('properties', OrderedDict([('dec', "*

 * *            "OrderedDict([('type', 'string'), ('description', 'Declination of the reference star, "*

 * *            "in a format understood by AstroPy'), (' […]*

```diff
@@ -47,38 +47,15 @@
                     "examples": [
                         "52arcsec",
                         "74.4arcsec"
                     ],
                     "type": "string"
                 },
                 "reference-star": {
-                    "additionalProperties": false,
-                    "properties": {
-                        "dec": {
-                            "description": "Declination of the reference star, in a format understood by AstroPy",
-                            "examples": [
-                                "-24d 5m 16s",
-                                "-15.967d"
-                            ],
-                            "type": "string"
-                        },
-                        "ra": {
-                            "description": "Right ascension of the reference star, in a format understood by AstroPy",
-                            "examples": [
-                                "23h 17m 22s",
-                                "134.9823d"
-                            ],
-                            "type": "string"
-                        }
-                    },
-                    "required": [
-                        "dec",
-                        "ra"
-                    ],
-                    "type": "object"
+                    "$ref": "#/$defs/reference-star"
                 }
             },
             "required": [
                 "bundle-separation"
             ],
             "type": "object"
         },
@@ -122,14 +99,40 @@
                 "ephemeris-stepsize",
                 "horizons-id",
                 "name",
                 "start-time"
             ],
             "type": "object"
         },
+        "reference-star": {
+            "additionalProperties": false,
+            "properties": {
+                "dec": {
+                    "description": "Declination of the reference star, in a format understood by AstroPy",
+                    "examples": [
+                        "-24d 5m 16s",
+                        "-15.967d"
+                    ],
+                    "type": "string"
+                },
+                "ra": {
+                    "description": "Right ascension of the reference star, in a format understood by AstroPy",
+                    "examples": [
+                        "23h 17m 22s",
+                        "134.9823d"
+                    ],
+                    "type": "string"
+                }
+            },
+            "required": [
+                "dec",
+                "ra"
+            ],
+            "type": "object"
+        },
         "rss": {
             "oneOf": [
                 {
                     "$ref": "#/$defs/rss-imaging"
                 },
                 {
                     "$ref": "#/$defs/rss-spectroscopy"
@@ -201,14 +204,17 @@
             "additionalProperties": false,
             "properties": {
                 "mode": {
                     "description": "The mode, which must be \"spectroscopy\"",
                     "pattern": "^spectroscopy$",
                     "type": "string"
                 },
+                "reference-star": {
+                    "$ref": "#/$defs/reference-star"
+                },
                 "slit-height": {
                     "description": "The slit height, in a format understood by AstroPy",
                     "examples": [
                         "8arcmin",
                         "4 arcmin"
                     ],
                     "type": "string"
```

### Comparing `imephu-0.3.0/src/imephu/service/horizons.py` & `imephu-0.4.0/src/imephu/service/horizons.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/service/survey.py` & `imephu-0.4.0/src/imephu/service/survey.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/src/imephu/utils.py` & `imephu-0.4.0/src/imephu/utils.py`

 * *Files identical despite different names*

### Comparing `imephu-0.3.0/PKG-INFO` & `imephu-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imephu
-Version: 0.3.0
+Version: 0.4.0
 Summary: Generate finder charts for astronomical observations.
 License: MIT
 Author: Southern African Large Telescope
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

