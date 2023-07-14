# Comparing `tmp/ome_types-0.4.0rc2.tar.gz` & `tmp/ome_types-0.4.0rc3.tar.gz`

## Comparing `ome_types-0.4.0rc2.tar` & `ome_types-0.4.0rc3.tar`

### file list

```diff
@@ -1,57 +1,65 @@
--rw-r--r--   0        0        0    16554 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/__init__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/__main__.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/_config.py
--rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/_generator.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/_transformer.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/_util.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/main.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/templates/class.jinja2
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/templates/docstrings.numpy.jinja2
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_autogen/templates/enum.jinja2
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/__init__.py
--rw-r--r--   0        0        0    17941 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_conversion.py
--rw-r--r--   0        0        0   285655 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/ome-2016-06.xsd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/py.typed
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/units.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_mixins/__init__.py
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_mixins/_base_type.py
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_mixins/_ids.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_mixins/_instrument.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_mixins/_kinded.py
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_mixins/_ome.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_mixins/_reference.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_mixins/_util.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/_mixins/_validators.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/model/__init__.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/model/_color.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/model/_converters.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/model/_shape_union.py
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/model/_structured_annotations.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/model/_user_sequence.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/model/simple_types.py
--rw-r--r--   0        0        0    51712 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2003-FC-to-2008-09.xsl
--rw-r--r--   0        0        0    33502 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2007-06-to-2008-09.xsl
--rw-r--r--   0        0        0    31797 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2008-02-to-2008-09.xsl
--rw-r--r--   0        0        0    67202 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2008-09-to-2009-09.xsl
--rw-r--r--   0        0        0    18678 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2009-09-to-2010-04.xsl
--rw-r--r--   0        0        0    10744 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2010-04-to-2010-06.xsl
--rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2010-06-to-2011-06.xsl
--rw-r--r--   0        0        0    21773 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2011-06-to-2012-06.xsl
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2012-06-to-2013-06.xsl
--rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2013-06-to-2015-01.xsl
--rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/ome_types/transforms/2015-01-to-2016-06.xsl
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/__init__.py
--rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/bindings.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/compat.py
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/hooks/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/hooks/class_type.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/hooks/cli.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/LICENSE
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/README.md
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/hatch_build.py
--rw-r--r--   0        0        0     6296 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/pyproject.toml
--rw-r--r--   0        0        0    10223 2020-02-02 00:00:00.000000 ome_types-0.4.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    16554 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/__main__.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/_config.py
+-rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/_generator.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/_transformer.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/_util.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/main.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/templates/class.jinja2
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/templates/docstrings.numpy.jinja2
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_autogen/templates/enum.jinja2
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/__init__.py
+-rw-r--r--   0        0        0    17998 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_conversion.py
+-rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_pydantic_compat.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/napari.yaml
+-rw-r--r--   0        0        0   285655 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/ome-2016-06.xsd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/py.typed
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/units.py
+-rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/widget.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_mixins/__init__.py
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_mixins/_base_type.py
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_mixins/_ids.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_mixins/_instrument.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_mixins/_kinded.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_mixins/_ome.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_mixins/_reference.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_mixins/_util.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_mixins/_validators.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_vendor/__init__.py
+-rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_vendor/_pydantic_color_v1.py
+-rw-r--r--   0        0        0    21521 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/_vendor/_pydantic_color_v2.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/model/__init__.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/model/_color.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/model/_converters.py
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/model/_shape_union.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/model/_structured_annotations.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/model/_user_sequence.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/model/simple_types.py
+-rw-r--r--   0        0        0    51712 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2003-FC-to-2008-09.xsl
+-rw-r--r--   0        0        0    33502 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2007-06-to-2008-09.xsl
+-rw-r--r--   0        0        0    31797 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2008-02-to-2008-09.xsl
+-rw-r--r--   0        0        0    67202 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2008-09-to-2009-09.xsl
+-rw-r--r--   0        0        0    18678 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2009-09-to-2010-04.xsl
+-rw-r--r--   0        0        0    10744 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2010-04-to-2010-06.xsl
+-rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2010-06-to-2011-06.xsl
+-rw-r--r--   0        0        0    21773 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2011-06-to-2012-06.xsl
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2012-06-to-2013-06.xsl
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2013-06-to-2015-01.xsl
+-rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/ome_types/transforms/2015-01-to-2016-06.xsl
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/__init__.py
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/bindings.py
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/compat.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/config.py
+-rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/py.typed
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/pydantic_compat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/hooks/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/hooks/class_type.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/hooks/cli.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/LICENSE
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/README.md
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/hatch_build.py
+-rw-r--r--   0        0        0     6397 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/pyproject.toml
+-rw-r--r--   0        0        0    10335 2020-02-02 00:00:00.000000 ome_types-0.4.0rc3/PKG-INFO
```

### Comparing `ome_types-0.4.0rc2/CHANGELOG.md` & `ome_types-0.4.0rc3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_autogen/_config.py` & `ome_types-0.4.0rc3/src/ome_autogen/_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from __future__ import annotations
 
+import os
+
 from xsdata.codegen.writer import CodeWriter
 from xsdata.models import config as cfg
 from xsdata.utils import text
 
 from ome_autogen._generator import OmeGenerator
 from ome_autogen._util import camel_to_snake
+from xsdata_pydantic_basemodel.config import GeneratorOutput
 
-KindedTypes = "(Shape|ManufacturerSpec|Annotation)"
-
-
+PYDANTIC_SUPPORT = os.getenv("PYDANTIC_SUPPORT", "both")
+ALLOW_RESERVED_NAMES = {"type", "Type", "Union"}
+OME_FORMAT = "OME"
 MIXIN_MODULE = "ome_types._mixins"
 MIXINS: list[tuple[str, str, bool]] = [
     (".*", f"{MIXIN_MODULE}._base_type.OMEType", False),  # base type on every class
     ("OME", f"{MIXIN_MODULE}._ome.OMEMixin", True),
     ("Instrument", f"{MIXIN_MODULE}._instrument.InstrumentMixin", False),
     ("Reference", f"{MIXIN_MODULE}._reference.ReferenceMixin", True),
-    (KindedTypes, f"{MIXIN_MODULE}._kinded.KindMixin", True),
+    ("(Shape|ManufacturerSpec|Annotation)", f"{MIXIN_MODULE}._kinded.KindMixin", True),
 ]
 
-ALLOW_RESERVED_NAMES = {"type", "Type", "Union"}
-OME_FORMAT = "OME"
-
 
 def get_config(
     package: str, kw_only: bool = True, compound_fields: bool = False
 ) -> cfg.GeneratorConfig:
     # ALLOW "type" to be used as a field name
     text.stop_words.difference_update(ALLOW_RESERVED_NAMES)
 
@@ -47,21 +47,23 @@
                 import_string=import_string,
                 prepend=prepend,
             )
         )
 
     keep_case = cfg.NameConvention(cfg.NameCase.ORIGINAL, "type")
     return cfg.GeneratorConfig(
-        output=cfg.GeneratorOutput(
+        output=GeneratorOutput(
             package=package,
             # format.value lets us use our own generator
             # kw_only is important, it makes required fields actually be required
             format=cfg.OutputFormat(value=OME_FORMAT, kw_only=kw_only),
             structure_style=cfg.StructureStyle.CLUSTERS,
             docstring_style=cfg.DocstringStyle.NUMPY,
             compound_fields=cfg.CompoundFields(enabled=compound_fields),
+            # whether to create models that work for both pydantic 1 and 2
+            pydantic_support=PYDANTIC_SUPPORT,  # type: ignore
         ),
         # Add our mixins
         extensions=cfg.GeneratorExtensions(mixins),
         # Don't convert things like XMLAnnotation to XmlAnnotation
         conventions=cfg.GeneratorConventions(class_name=keep_case),
     )
```

### Comparing `ome_types-0.4.0rc2/src/ome_autogen/_generator.py` & `ome_types-0.4.0rc3/src/ome_autogen/_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,27 +25,27 @@
 # Methods and/or validators to add to generated classes
 # (predicate, method) where predicate returns True if the method should be added
 # to the given class.  Note: imports for these methods are added in
 # IMPORT_PATTERNS below.
 ADDED_METHODS: list[tuple[Callable[[Class], bool], str]] = [
     (
         lambda c: c.name == "BinData",
-        "\n\n_v = root_validator(pre=True)(bin_data_root_validator)",
+        "\n\n_vbindata = model_validator(mode='before')(bin_data_root_validator)",
     ),
     (
         lambda c: c.name == "Value",
-        "\n\n_v = validator('any_elements', each_item=True)(any_elements_validator)",
+        "\n\n_vany = field_validator('any_elements')(any_elements_validator)",
     ),
     (
         lambda c: c.name == "Pixels",
-        "\n\n_v = root_validator(pre=True)(pixels_root_validator)",
+        "\n\n_vpix = model_validator(mode='before')(pixels_root_validator)",
     ),
     (
         lambda c: c.name == "XMLAnnotation",
-        "\n\n_v = validator('value', pre=True)(xml_value_validator)",
+        "\n\n_vval = field_validator('value', mode='before')(xml_value_validator)",
     ),
     (
         lambda c: c.name == "PixelType",
         "\n\nnumpy_dtype = property(pixel_type_to_numpy_dtype)",
     ),
 ]
 
@@ -82,14 +82,18 @@
     for o in CLASS_OVERRIDES
     if o.module_name
 }
 IMPORT_PATTERNS.update(
     {
         "ome_types._mixins._util": {"new_uuid": ["default_factory=new_uuid"]},
         "datetime": {"datetime": ["datetime"]},
+        "ome_types._pydantic_compat": {
+            "model_validator": ["model_validator("],
+            "field_validator": ["field_validator("],
+        },
         "ome_types._mixins._validators": {
             "any_elements_validator": ["any_elements_validator"],
             "bin_data_root_validator": ["bin_data_root_validator"],
             "pixels_root_validator": ["pixels_root_validator"],
             "xml_value_validator": ["xml_value_validator"],
             "pixel_type_to_numpy_dtype": ["pixel_type_to_numpy_dtype"],
         },
@@ -230,15 +234,14 @@
 
     @classmethod
     def build_import_patterns(cls) -> dict[str, dict]:
         patterns = super().build_import_patterns()
         patterns.setdefault("pydantic", {}).update(
             {
                 "validator": ["validator("],
-                "root_validator": ["root_validator("],
             }
         )
         patterns.update(IMPORT_PATTERNS)
         return {key: patterns[key] for key in sorted(patterns)}
 
     def field_default_value(self, attr: Attr, ns_map: dict | None = None) -> str:
         if attr.tag == "Attribute" and attr.name == "ID":
```

### Comparing `ome_types-0.4.0rc2/src/ome_autogen/_transformer.py` & `ome_types-0.4.0rc3/src/ome_autogen/_transformer.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_autogen/_util.py` & `ome_types-0.4.0rc3/src/ome_autogen/_util.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_autogen/main.py` & `ome_types-0.4.0rc3/src/ome_autogen/main.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_autogen/templates/class.jinja2` & `ome_types-0.4.0rc3/src/ome_autogen/templates/class.jinja2`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_autogen/templates/enum.jinja2` & `ome_types-0.4.0rc3/src/ome_autogen/templates/enum.jinja2`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_types/__init__.py` & `ome_types-0.4.0rc3/src/ome_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_types/_conversion.py` & `ome_types-0.4.0rc3/src/ome_types/_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from pathlib import Path
 from struct import Struct
 from typing import TYPE_CHECKING, cast, overload
 
 from pydantic import BaseModel
 from xsdata.formats.dataclass.parsers.config import ParserConfig
 
+from ome_types._pydantic_compat import model_dump
 from xsdata_pydantic_basemodel.bindings import (
     SerializerConfig,
     XmlParser,
     XmlSerializer,
 )
 
 try:
@@ -205,15 +206,15 @@
 
     Returns
     -------
     dict[str, Any]
         A dictionary representation of the OME object or XML document.
     """
     if isinstance(source, BaseModel):
-        return source.dict(exclude_defaults=True)
+        return model_dump(source, exclude_defaults=True)
 
     return from_xml(  # type: ignore[return-value]
         source,
         # the class_factory is what prevents class instantiation,
         # simply returning the params instead
         parser_kwargs={"config": ParserConfig(class_factory=lambda a, b: b)},
     )
```

### Comparing `ome_types-0.4.0rc2/src/ome_types/ome-2016-06.xsd` & `ome_types-0.4.0rc3/src/ome_types/ome-2016-06.xsd`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_types/units.py` & `ome_types-0.4.0rc3/src/ome_types/units.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,10 +44,13 @@
 def add_quantity_properties(cls: type[BaseModel]) -> None:
     """Add quantity properties to each field with a corresponding *_unit field.
 
     Quantity properties allow you to access the value and unit of a field in a single
     X_quantity property, where X is the name of the field.  It returns a pint object.
     """
     _QUANTITY_FIELD = "{}_quantity"
-    for field in cls.__fields__:
-        if _UNIT_FIELD.format(field) in cls.__fields__:
+    # for some odd reason, cls.model_fields isn't always ready to go yet at this point
+    # only in pydantic2... so use __annotations__ instead
+    field_names = set(cls.__annotations__)
+    for field in field_names:
+        if _UNIT_FIELD.format(field) in field_names:
             setattr(cls, _QUANTITY_FIELD.format(field), _quantity_property(field))
```

### Comparing `ome_types-0.4.0rc2/src/ome_types/_mixins/_base_type.py` & `ome_types-0.4.0rc3/src/ome_types/_mixins/_base_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,34 +3,43 @@
 from enum import Enum
 from textwrap import indent
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     Dict,
-    MutableSequence,
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
-from pydantic import BaseModel, validator
+from pydantic import BaseModel
 
 from ome_types._mixins._ids import validate_id
+from ome_types._pydantic_compat import (
+    PYDANTIC2,
+    field_type,
+    field_validator,
+    model_dump,
+    model_fields,
+    update_set_fields,
+)
 
 try:
     from ome_types.units import add_quantity_properties
 except ImportError:
     add_quantity_properties = lambda cls: None  # noqa: E731
 
 if TYPE_CHECKING:
+    from pydantic import ConfigDict
+
     from ome_types._conversion import XMLSource
 
 
 T = TypeVar("T", bound="OMEType")
 # Default value to support automatic numbering for id field values.
 AUTO_SEQUENCE = "__auto_sequence__"
 
@@ -64,42 +73,50 @@
             warnings.warn(
                 f"Field {key!r} is deprecated. Use {DEPRECATED_NAMES[key]!r} instead.",
                 stacklevel=2,
             )
             data[DEPRECATED_NAMES[key]] = data.pop(key)
 
 
+CONFIG: "ConfigDict" = {
+    "arbitrary_types_allowed": True,
+    "validate_assignment": True,
+    "validate_default": True,
+}
+
+
 class OMEType(BaseModel):
     """The base class that all OME Types inherit from.
 
     This provides some global conveniences around auto-setting ids. (i.e., making them
     optional in the class constructor, but never `None` after initialization.).
     It provides a nice `__repr__` that hides things that haven't been changed from
     defaults.  It adds ``*_quantity`` property for fields that have both a value and a
     unit, where `*_quantity` is a [`pint.Quantity`][].  It also provides pickling
     support.
     """
 
     # pydantic BaseModel configuration.
     # see: https://pydantic-docs.helpmanual.io/usage/model_config/
-    class Config:
-        arbitrary_types_allowed = False
-        validate_assignment = True
-        underscore_attrs_are_private = True
-        use_enum_values = False
-        validate_all = True
+
+    if PYDANTIC2:
+        model_config = CONFIG
+    else:
+        Config = type("Config", (), CONFIG)  # type: ignore
 
     # allow use with weakref
     __slots__: ClassVar[Set[str]] = {"__weakref__"}  # type: ignore
 
-    _v = validator("id", pre=True, always=True, check_fields=False)(validate_id)
+    _vid = field_validator("id", mode="before", always=True, check_fields=False)(
+        validate_id
+    )
 
     def __init__(self, **data: Any) -> None:
         warn_extra = data.pop("warn_extra", True)
-        field_names = set(self.__fields__.keys())
+        field_names = set(model_fields(self))
         _move_deprecated_fields(data, field_names)
         super().__init__(**data)
         kwargs = set(data.keys())
         extra = kwargs - field_names
         if extra and warn_extra:
             warnings.warn(
                 f"Unrecognized fields for type {type(self)}: {kwargs - field_names}",
@@ -112,22 +129,25 @@
         where `*_quantity` is a pint `Quantity`.
         """
         add_quantity_properties(cls)
 
     def __repr_args__(self) -> Sequence[Tuple[Optional[str], Any]]:
         """Repr with only set values, and truncated sequences."""
         args = []
-        for k, v in self._iter(exclude_defaults=True):
+        for k, v in model_dump(self, exclude_defaults=True).items():
+            if k == "kind":
+                continue
             if isinstance(v, Sequence) and not isinstance(v, str):
                 if v == []:  # skip empty lists
                     continue
                 # if this is a sequence with a long repr, just show the length
                 # and type
                 if len(repr(v).split(",")) > 5:
-                    type_name = self.__fields__[k].type_.__name__
+                    ftype = field_type(model_fields(self)[k])
+                    type_name = getattr(field_type, "__name__", str(ftype))
                     v = _RawRepr(f"[<{len(v)} {type_name}>]")
             elif isinstance(v, Enum):
                 v = v.value
             elif isinstance(v, datetime):
                 v = v.isoformat()
             args.append((k, v))
         return sorted(args, key=lambda f: f[0] not in ("name", "id"))
@@ -149,15 +169,16 @@
             new_key = DEPRECATED_NAMES[key]
             warnings.warn(
                 f"Attribute '{cls_name}.{key}' is deprecated, use {new_key!r} instead",
                 DeprecationWarning,
                 stacklevel=2,
             )
             return getattr(self, new_key)
-        raise AttributeError(f"{cls_name} object has no attribute {key!r}")
+
+        return super().__getattr__(key)  # type: ignore
 
     def to_xml(self, **kwargs: Any) -> str:
         """Serialize this object to XML.
 
         See docstring of [`ome_types.to_xml`][] for kwargs.
         """
         from ome_types._conversion import to_xml
@@ -183,26 +204,15 @@
         """Update set fields with populated mutable sequences.
 
         Because pydantic isn't aware of mutations to sequences, it can't tell when
         a field has been "set" by mutating a sequence.  This method updates the
         self.__fields_set__ attribute to reflect that.  We assume that if an attribute
         is not None, and is not equal to the default value, then it has been set.
         """
-        for field_name, field in self.__fields__.items():
-            current = getattr(self, field_name)
-            if not current:
-                continue
-            if current != field.get_default():
-                self.__fields_set__.add(field_name)
-            if isinstance(current, OMEType):
-                current._update_set_fields()
-            if isinstance(current, MutableSequence):
-                for item in current:
-                    if isinstance(item, OMEType):
-                        item._update_set_fields()
+        update_set_fields(self)
 
 
 class _RawRepr:
     """Helper class to allow repr to show raw values for fields that are sequences."""
 
     def __init__(self, raw: str) -> None:
         self.raw = raw
```

### Comparing `ome_types-0.4.0rc2/src/ome_types/_mixins/_ids.py` & `ome_types-0.4.0rc3/src/ome_types/_mixins/_ids.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import re
 import warnings
 from contextlib import suppress
 from typing import TYPE_CHECKING, Any, cast
 
+from ome_types._pydantic_compat import field_regex
+
 if TYPE_CHECKING:
     from pydantic import BaseModel
     from typing_extensions import Final
 
 # Default value to support automatic numbering for id field values.
 AUTO_SEQUENCE: Final = "__auto_sequence__"
 # map of id_name -> max id value
@@ -19,18 +21,16 @@
 # is unique to each OME instance
 CONVERTED_IDS: dict[tuple[str, str], str] = {}
 
 
 def _get_id_name_and_pattern(cls: type[BaseModel]) -> tuple[str, str]:
     # let this raise if it doesn't exist...
     # this should only be used on classes that have an id field
-    id_field = cls.__fields__["id"]
-    id_pattern = cast(str, id_field.field_info.regex)
+    id_pattern = cast(str, field_regex(cls, "id"))
     id_name = id_pattern.split(":")[-3]
-
     return id_name, id_pattern
 
 
 def validate_id(cls: type[BaseModel], value: int | str) -> Any:
     """Pydantic validator for ID fields in OME models.
 
     This validator does the following:
```

### Comparing `ome_types-0.4.0rc2/src/ome_types/_mixins/_instrument.py` & `ome_types-0.4.0rc3/src/ome_types/_mixins/_instrument.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_types/_mixins/_ome.py` & `ome_types-0.4.0rc3/src/ome_types/_mixins/_ome.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import warnings
 import weakref
 from typing import TYPE_CHECKING, Any, BinaryIO, Sequence
 
 from ome_types._mixins._base_type import OMEType
 from ome_types._mixins._ids import CONVERTED_IDS
+from ome_types._pydantic_compat import model_fields
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from ome_types._autogenerated.ome_2016_06 import OME, Reference
 
 
@@ -55,15 +56,15 @@
     from ome_types.model import Reference
 
     ids: dict[str, OMEType] = {}
     if isinstance(value, Sequence) and not isinstance(value, str):
         for v in value:
             ids.update(collect_ids(v))
     elif isinstance(value, OMEType):
-        for fname in value.__fields__:
+        for fname in model_fields(value):
             if fname == "id" and not isinstance(value, Reference):
                 # We don't need to recurse on the id string, so just record it
                 # and move on.
                 ids[value.id] = value
             else:
                 ids.update(collect_ids(getattr(value, fname)))
     # Do nothing for uninteresting types.
@@ -83,11 +84,11 @@
     references: list[Reference] = []
     if isinstance(value, Reference):
         references.append(value)
     elif isinstance(value, list):
         for v in value:
             references.extend(collect_references(v))
     elif isinstance(value, OMEType):
-        for f in value.__fields__:
+        for f in model_fields(value):
             references.extend(collect_references(getattr(value, f)))
     # Do nothing for uninteresting types
     return references
```

### Comparing `ome_types-0.4.0rc2/src/ome_types/_mixins/_reference.py` & `ome_types-0.4.0rc3/src/ome_types/_mixins/_reference.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import weakref
 from typing import Any, Dict, Optional, Union
 
+from pydantic import PrivateAttr
+
 from ome_types._mixins._base_type import OMEType
 
 
 class ReferenceMixin(OMEType):
-    _ref: Optional[weakref.ReferenceType] = None
+    _ref: Optional[weakref.ReferenceType] = PrivateAttr(None)
 
     @property
     def ref(self) -> Union[OMEType, None]:
         if self._ref is None:
             raise ValueError("references not yet resolved on root OME object")
         return self._ref()
 
     def __getstate__(self: Any) -> Dict[str, Any]:
         """Support pickle of our weakref references."""
         state = super().__getstate__()
-        state["__private_attribute_values__"].pop("_ref", None)
+        if "__private_attribute_values__" in state:
+            state["__private_attribute_values__"].pop("_ref", None)
+        elif "__pydantic_private__" in state:
+            state["__pydantic_private__"].pop("_ref", None)
         return state
```

### Comparing `ome_types-0.4.0rc2/src/ome_types/_mixins/_validators.py` & `ome_types-0.4.0rc3/src/ome_types/_mixins/_validators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """These validators are added to the generated classes in ome_types._autogenerated.
 
 that logic is in the `methods` method in ome_autogen/_generator.py
 """
 import warnings
-from typing import TYPE_CHECKING, Any, Dict
+from typing import TYPE_CHECKING, Any, Dict, List, Sequence
 
 if TYPE_CHECKING:
     from ome_types.model import (  # type: ignore
         BinData,
         Pixels,
         PixelType,
         XMLAnnotation,
@@ -27,39 +27,41 @@
                 "BinData length is non-zero but value is missing", stacklevel=2
             )
         values["value"] = b""
     return values
 
 
 # @root_validator(pre=True)
-def pixels_root_validator(cls: "Pixels", values: dict) -> dict:
-    if "metadata_only" in values:
-        if isinstance(values["metadata_only"], bool):
-            if not values["metadata_only"]:
-                values.pop("metadata_only")
+def pixels_root_validator(cls: "Pixels", value: dict) -> dict:
+    if "metadata_only" in value:
+        if isinstance(value["metadata_only"], bool):
+            if not value["metadata_only"]:
+                value.pop("metadata_only")
             else:
                 # type ignore in case the autogeneration hasn't been built
                 from ome_types.model import MetadataOnly  # type: ignore
 
-                values["metadata_only"] = MetadataOnly()
+                value["metadata_only"] = MetadataOnly()
 
-    return values
+    return value
 
 
-# @validator("any_elements", each_item=True)
-def any_elements_validator(cls: "XMLAnnotation.Value", v: Any) -> "AnyElement":
+# @validator("any_elements")
+def any_elements_validator(
+    cls: "XMLAnnotation.Value", v: List[Any]
+) -> List["AnyElement"]:
     # This validator is used because XMLAnnotation.Value.any_elements is
     # annotated as List[object]. So pydantic won't coerce dicts to AnyElement
     # automatically (which is important when constructing OME objects from dicts)
-    if isinstance(v, dict):
-        # this needs to be delayed until runtime because of circular imports
-        from xsdata_pydantic_basemodel.compat import AnyElement
+    if not isinstance(v, Sequence):
+        raise ValueError(f"any_elements must be a sequence, not {type(v)}")
+    # this needs to be delayed until runtime because of circular imports
+    from xsdata_pydantic_basemodel.compat import AnyElement
 
-        return AnyElement(**v)
-    return v
+    return [AnyElement(**v) if isinstance(v, dict) else v for v in v]
 
 
 # @validator('value', pre=True)
 def xml_value_validator(cls: "XMLAnnotation", v: Any) -> "XMLAnnotation.Value":
     if isinstance(v, str):
         # FIXME: this is a hack to support passing a string to XMLAnnotation.value
         # there must be a more direct way to do this...
```

### Comparing `ome_types-0.4.0rc2/src/ome_types/model/__init__.py` & `ome_types-0.4.0rc3/src/ome_types/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_types/model/_color.py` & `ome_types-0.4.0rc3/src/ome_types/model/_color.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from contextlib import suppress
 from typing import Tuple, Union
 
-from pydantic import color
+from ome_types._vendor import Color as _Color
 
 __all__ = ["Color"]
 
 RGBA = Tuple[int, int, int, float]
 ColorType = Union[Tuple[int, int, int], RGBA, str, int]
 
 
-class Color(color.Color):
+class Color(_Color):
     """A Pydantic Color subclass that converts to and from OME int32 types."""
 
     def __init__(self, val: ColorType = -1) -> None:
         with suppress(ValueError, TypeError):
             val = self._int2tuple(int(val))  # type: ignore
         super().__init__(val)  # type: ignore [arg-type]
```

### Comparing `ome_types-0.4.0rc2/src/ome_types/model/_converters.py` & `ome_types-0.4.0rc3/src/ome_types/model/_converters.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_types/model/simple_types.py` & `ome_types-0.4.0rc3/src/ome_types/model/simple_types.py`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_types/transforms/2003-FC-to-2008-09.xsl` & `ome_types-0.4.0rc3/src/ome_types/transforms/2003-FC-to-2008-09.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_types/transforms/2007-06-to-2008-09.xsl` & `ome_types-0.4.0rc3/src/ome_types/transforms/2007-06-to-2008-09.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_types/transforms/2008-02-to-2008-09.xsl` & `ome_types-0.4.0rc3/src/ome_types/transforms/2008-02-to-2008-09.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_types/transforms/2008-09-to-2009-09.xsl` & `ome_types-0.4.0rc3/src/ome_types/transforms/2008-09-to-2009-09.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_types/transforms/2009-09-to-2010-04.xsl` & `ome_types-0.4.0rc3/src/ome_types/transforms/2009-09-to-2010-04.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_types/transforms/2010-04-to-2010-06.xsl` & `ome_types-0.4.0rc3/src/ome_types/transforms/2010-04-to-2010-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_types/transforms/2010-06-to-2011-06.xsl` & `ome_types-0.4.0rc3/src/ome_types/transforms/2010-06-to-2011-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_types/transforms/2011-06-to-2012-06.xsl` & `ome_types-0.4.0rc3/src/ome_types/transforms/2011-06-to-2012-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_types/transforms/2012-06-to-2013-06.xsl` & `ome_types-0.4.0rc3/src/ome_types/transforms/2012-06-to-2013-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_types/transforms/2013-06-to-2015-01.xsl` & `ome_types-0.4.0rc3/src/ome_types/transforms/2013-06-to-2015-01.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/ome_types/transforms/2015-01-to-2016-06.xsl` & `ome_types-0.4.0rc3/src/ome_types/transforms/2015-01-to-2016-06.xsl`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/bindings.py` & `ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/bindings.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from xsdata.formats.dataclass import context, parsers, serializers
 from xsdata.formats.dataclass.serializers import config
 from xsdata.formats.dataclass.serializers.mixins import XmlWriterEvent
 from xsdata.models.enums import QNames
 from xsdata.utils import collections, namespaces
 from xsdata.utils.constants import EMPTY_MAP, return_input
 
+from xsdata_pydantic_basemodel.pydantic_compat import fields_set
+
 if TYPE_CHECKING:
     from pydantic import BaseModel
     from xsdata.formats.dataclass.models.elements import XmlMeta
 
 
 class XmlContext(context.XmlContext):
     """Pydantic BaseModel ready xml context instance."""
@@ -88,15 +90,15 @@
             ignore_unset,
             getattr(self.config, "attribute_sort_key", None),
         ):
             yield XmlWriterEvent.ATTR, key, value
 
         for var, value in self.next_value(obj, meta):
             # XXX: reason 2 for overriding.
-            if ignore_unset and var.name not in obj.__fields_set__:
+            if ignore_unset and var.name not in fields_set(obj):
                 continue
             yield from self.write_value(value, var, namespace)
 
         yield XmlWriterEvent.END, qname
 
     # overriding so we can implement support for `ignore_unset_attributes`
     # and so that we can sort attributes as we want
@@ -120,15 +122,15 @@
         :param nillable: Is model nillable
         :param xsi_type: The true xsi:type of the object
         :param ignore_optionals: Skip optional attributes with default
             value
         :return:
         """
 
-        set_fields = obj.__fields_set__ if ignore_unset else set()
+        set_fields = fields_set(obj) if ignore_unset else set()
         vars_ = meta.get_attribute_vars()
         if attribute_sort_key is not None:
             vars_ = sorted(meta.get_attribute_vars(), key=attribute_sort_key)
 
         # ^^^ new
 
         for var in vars_:
@@ -137,15 +139,14 @@
                 if (
                     value is None
                     or (collections.is_array(value) and not value)
                     or (ignore_optionals and var.is_optional(value))
                     or (ignore_unset and var.name not in set_fields)  # new
                 ):
                     continue
-
                 yield var.qname, cls.encode(value, var)
             else:
                 yield from getattr(obj, var.name, EMPTY_MAP).items()
 
         if xsi_type:
             yield QNames.XSI_TYPE, QName(xsi_type)
```

### Comparing `ome_types-0.4.0rc2/src/xsdata_pydantic_basemodel/compat.py` & `ome_types-0.4.0rc3/src/xsdata_pydantic_basemodel/compat.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,44 @@
+from typing import Any, Callable, Dict, Generic, List, Optional, Tuple, Type, TypeVar
+
 try:
     from lxml import etree as ET
 except ImportError:
     import xml.etree.ElementTree as ET  # type: ignore
 
-from dataclasses import MISSING, field
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Generic,
-    List,
-    Optional,
-    Tuple,
-    Type,
-    TypeVar,
-    cast,
-)
-
 from pydantic import BaseModel, validators
-from pydantic.fields import Field, ModelField, Undefined
 from xsdata.formats.dataclass.compat import Dataclasses, class_types
 from xsdata.formats.dataclass.models.elements import XmlType
 from xsdata.models.datatype import XmlDate, XmlDateTime, XmlDuration, XmlPeriod, XmlTime
 
+from xsdata_pydantic_basemodel.pydantic_compat import (
+    PYDANTIC2,
+    Field,
+    dataclass_fields,
+    model_config,
+    update_forward_refs,
+)
+
 T = TypeVar("T", bound=object)
 
 
+# don't switch to exclude ... it makes it hard to add fields to the
+# schema without breaking backwards compatibility
+_config = model_config(arbitrary_types_allowed=True)
+
+
+class _BaseModel(BaseModel):
+    """Base model for all types."""
+
+    if PYDANTIC2:
+        model_config = _config  # type: ignore
+    else:
+        Config = _config  # type: ignore
+
+
 class AnyElement(BaseModel):
     """Generic model to bind xml document data to wildcard fields.
 
     :param qname: The element's qualified name
     :param text: The element's text content
     :param tail: The element's tail content
     :param children: The element's list of child elements.
@@ -42,16 +51,18 @@
     children: List["AnyElement"] = Field(
         default_factory=list, metadata={"type": XmlType.WILDCARD}
     )
     attributes: Dict[str, str] = Field(
         default_factory=dict, metadata={"type": XmlType.ATTRIBUTES}
     )
 
-    class Config:
-        arbitrary_types_allowed = True
+    if PYDANTIC2:
+        model_config = _config  # type: ignore
+    else:
+        Config = _config  # type: ignore
 
     def to_etree_element(self) -> "ET._Element":
         elem = ET.Element(self.qname or "", self.attributes)
         elem.text = self.text
         elem.tail = self.tail
         for child in self.children:
             elem.append(child.to_etree_element())
@@ -68,64 +79,39 @@
     :param type: The real xsi:type
     """
 
     qname: str
     value: T
     type: Optional[str] = None
 
-    class Config:
-        arbitrary_types_allowed = True
+    if PYDANTIC2:
+        model_config = _config  # type: ignore
+    else:
+        Config = _config  # type: ignore
 
 
 class PydanticBaseModel(Dataclasses):
     @property
     def any_element(self) -> Type:
         return AnyElement
 
     @property
     def derived_element(self) -> Type:
         return DerivedElement
 
     def is_model(self, obj: Any) -> bool:
         clazz = obj if isinstance(obj, type) else type(obj)
         if issubclass(clazz, BaseModel):
-            clazz.update_forward_refs()
+            update_forward_refs(clazz)
             return True
 
         return False
 
     def get_fields(self, obj: Any) -> Tuple[Any, ...]:
-        _fields = cast("BaseModel", obj).__fields__.values()
-        return tuple(_pydantic_field_to_dataclass_field(field) for field in _fields)
-
-
-def _pydantic_field_to_dataclass_field(pydantic_field: ModelField) -> Any:
-    if pydantic_field.default_factory is not None:
-        default_factory: Any = pydantic_field.default_factory
-        default = MISSING
-    else:
-        default_factory = MISSING
-        default = (
-            MISSING
-            if pydantic_field.default in (Undefined, Ellipsis)
-            else pydantic_field.default
-        )
-
-    dataclass_field = field(  # type: ignore
-        default=default,
-        default_factory=default_factory,
-        # init=True,
-        # hash=None,
-        # compare=True,
-        metadata=pydantic_field.field_info.extra.get("metadata", {}),
-        # kw_only=MISSING,
-    )
-    dataclass_field.name = pydantic_field.name
-    dataclass_field.type = pydantic_field.type_
-    return dataclass_field
+        return tuple(dataclass_fields(obj))
 
 
 class_types.register("pydantic-basemodel", PydanticBaseModel())
 
 
 def make_validators(tp: Type, factory: Callable) -> List[Callable]:
     def validator(value: Any) -> Any:
@@ -136,26 +122,34 @@
             return factory(value)
 
         raise ValueError
 
     return [validator]
 
 
-if hasattr(validators, "_VALIDATORS"):
-    validators._VALIDATORS.extend(
-        [
-            (XmlDate, make_validators(XmlDate, XmlDate.from_string)),
-            (XmlDateTime, make_validators(XmlDateTime, XmlDateTime.from_string)),
-            (XmlTime, make_validators(XmlTime, XmlTime.from_string)),
-            (XmlDuration, make_validators(XmlDuration, XmlDuration)),
-            (XmlPeriod, make_validators(XmlPeriod, XmlPeriod)),
-            (ET.QName, make_validators(ET.QName, ET.QName)),
-        ]
-    )
+_validators = {
+    XmlDate: make_validators(XmlDate, XmlDate.from_string),
+    XmlDateTime: make_validators(XmlDateTime, XmlDateTime.from_string),
+    XmlTime: make_validators(XmlTime, XmlTime.from_string),
+    XmlDuration: make_validators(XmlDuration, XmlDuration),
+    XmlPeriod: make_validators(XmlPeriod, XmlPeriod),
+    ET.QName: make_validators(ET.QName, ET.QName),
+}
+
+if not PYDANTIC2:
+    validators._VALIDATORS.extend(list(_validators.items()))
 else:
-    import warnings
+    from pydantic import BaseModel
+    from pydantic_core import core_schema as cs
 
-    warnings.warn(
-        "Could not find pydantic.validators._VALIDATORS."
-        "xsdata-pydantic-basemodel may be incompatible with your pydantic version.",
-        stacklevel=2,
-    )
+    def _make_get_core_schema(validator: Callable) -> Callable:
+        def get_core_schema(*args: Any) -> cs.PlainValidatorFunctionSchema:
+            return cs.general_plain_validator_function(validator)
+
+        return get_core_schema
+
+    for type_, val in _validators.items():
+        get_schema = _make_get_core_schema(val[0])
+        try:
+            type_.__get_pydantic_core_schema__ = get_schema  # type: ignore
+        except TypeError as e:
+            print(e)
```

### Comparing `ome_types-0.4.0rc2/.gitignore` & `ome_types-0.4.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/LICENSE` & `ome_types-0.4.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/README.md` & `ome_types-0.4.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `ome_types-0.4.0rc2/pyproject.toml` & `ome_types-0.4.0rc3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -25,26 +25,26 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version"]
 dependencies = [
-  "pydantic <2.0",
+  "pydantic >=1.9.0",
   "xsdata >=23.5",                              # 23.6 necessary for codegen, but not for runtime
   "importlib_metadata; python_version < '3.8'",
 ]
 
 [project.urls]
 Source = "https://github.com/tlambert03/ome-types"
 Tracker = "https://github.com/tlambert03/ome-types/issues"
 Documentation = "https://ome-types.readthedocs.io/en/latest/"
 
-[project.entry-points."napari.plugin"]
-ome-types = "ome_types._napari_plugin"
+[project.entry-points."napari.manifest"]
+ome-types = "ome_types:napari.yaml"
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
 pint = ["Pint >=0.15"]
 lxml = ["lxml >=4.8.0"]
 dev = [
@@ -62,14 +62,15 @@
   "pint",
   "pytest-codspeed",
   "pytest-cov",
   "pytest-mypy-plugins",
   "pytest",
   "xmlschema",
 ]
+test-qt = ["qtpy", "pytest-qt"]
 
 # https://hatch.pypa.io/latest/plugins/build-hook/custom/
 [tool.hatch.build.targets.wheel.hooks.custom]
 # requirements to run the autogen script in hatch_build.py
 require-runtime-dependencies = true
 dependencies = ["black", "ruff", "xsdata[cli]>=23.6"]
 
@@ -121,15 +122,15 @@
   "D404",   # First word of the docstring should not be This
   "D413",   # Missing blank line after last section
   "D416",   # Section name should end with a colon
   "C901",   # Function is too complex
   "RUF009", # Do not perform function calls in default arguments
   "S3",     # xml security
 ]
-exclude = ['src/_ome_autogen.py']
+exclude = ['src/_ome_autogen.py', 'src/ome_types/_vendor']
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all" # Disallow all relative imports.
 
 [tool.ruff.per-file-ignores]
 "tests/*.py" = ["D", "S"]
 "src/ome_autogen.py" = ["D10", "E501"]
@@ -201,15 +202,15 @@
   "except ImportError",
   "\\.\\.\\.",
   "raise NotImplementedError()",
 ]
 
 [tool.coverage.run]
 source = ["ome_types", "ome_autogen"]
-omit = ["src/ome_types/_autogenerated/*", "/private/var/folders/*"]
+omit = ["src/ome_types/_autogenerated/*", "/private/var/folders/*", "*/_vendor/*", "src/ome_types/widget.py"]
 
 # Entry points -- REMOVE ONCE XSDATA-PYDANTIC-BASEMODEL IS SEPARATE
 [project.entry-points."xsdata.plugins.class_types"]
 xsdata_pydantic_basemodel = "xsdata_pydantic_basemodel.hooks.class_type"
 
 [project.entry-points."xsdata.plugins.cli"]
 xsdata_pydantic_basemodel = "xsdata_pydantic_basemodel.hooks.cli"
```

### Comparing `ome_types-0.4.0rc2/PKG-INFO` & `ome_types-0.4.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ome-types
-Version: 0.4.0rc2
+Version: 0.4.0rc3
 Summary: Python dataclasses for the OME data model
 Project-URL: Source, https://github.com/tlambert03/ome-types
 Project-URL: Tracker, https://github.com/tlambert03/ome-types/issues
 Project-URL: Documentation, https://ome-types.readthedocs.io/en/latest/
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: MIT
 License-File: LICENSE
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata; python_version < '3.8'
-Requires-Dist: pydantic<2.0
+Requires-Dist: pydantic>=1.9.0
 Requires-Dist: xsdata>=23.5
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: types-lxml; python_version >= '3.8' and extra == 'dev'
@@ -45,14 +45,17 @@
 Requires-Dist: numpy; extra == 'test'
 Requires-Dist: pint; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-codspeed; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-mypy-plugins; extra == 'test'
 Requires-Dist: xmlschema; extra == 'test'
+Provides-Extra: test-qt
+Requires-Dist: pytest-qt; extra == 'test-qt'
+Requires-Dist: qtpy; extra == 'test-qt'
 Description-Content-Type: text/markdown
 
 # ome-types
 
 [![License](https://img.shields.io/github/license/tlambert03/ome-types)](LICENSE)
 [![Version](https://img.shields.io/pypi/v/ome-types.svg)](https://pypi.python.org/pypi/ome-types)
 [![CondaVersion](https://img.shields.io/conda/v/conda-forge/ome-types)](https://anaconda.org/conda-forge/ome-types)
```

