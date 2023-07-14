# Comparing `tmp/q2report-0.1.29.tar.gz` & `tmp/q2report-0.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2report-0.1.29.tar", max compression
+gzip compressed data, was "q2report-0.1.30.tar", max compression
```

## Comparing `q2report-0.1.29.tar` & `q2report-0.1.30.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2report-0.1.29/LICENSE
--rw-r--r--   0        0        0      536 2023-07-08 21:36:37.928411 q2report-0.1.29/pyproject.toml
--rw-r--r--   0        0        0       42 2022-12-11 17:39:38.103740 q2report-0.1.29/q2report/__init__.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:38.103740 q2report-0.1.29/q2report/q2engine/__init__.py
--rw-r--r--   0        0        0      115 2022-12-11 17:39:38.103740 q2report-0.1.29/q2report/q2engine/q2engine_core.py
--rw-r--r--   0        0        0       90 2022-12-11 17:39:38.107739 q2report-0.1.29/q2report/q2engine/q2engine_pyqt.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:38.107739 q2report-0.1.29/q2report/q2printer/__init__.py
--rw-r--r--   0        0        0     8678 2023-06-21 10:36:17.872724 q2report-0.1.29/q2report/q2printer/docx_parts.py
--rw-r--r--   0        0        0     8479 2023-06-25 22:47:50.666231 q2report-0.1.29/q2report/q2printer/q2printer.py
--rw-r--r--   0        0        0    18820 2023-06-28 08:23:20.140407 q2report-0.1.29/q2report/q2printer/q2printer_docx.py
--rw-r--r--   0        0        0     6126 2023-06-21 17:49:50.189551 q2report-0.1.29/q2report/q2printer/q2printer_html.py
--rw-r--r--   0        0        0    20678 2023-06-21 17:49:55.953006 q2report-0.1.29/q2report/q2printer/q2printer_xlsx.py
--rw-r--r--   0        0        0     8792 2023-06-21 10:36:28.504330 q2report-0.1.29/q2report/q2printer/xlsx_parts.py
--rw-r--r--   0        0        0    30080 2023-07-08 20:20:24.915617 q2report-0.1.29/q2report/q2report.py
--rw-r--r--   0        0        0     1708 2023-02-10 16:01:23.063515 q2report-0.1.29/q2report/q2utils.py
--rw-r--r--   0        0        0       22 2023-07-08 21:36:40.175773 q2report-0.1.29/q2report/version.py
--rw-r--r--   0        0        0     1486 2022-12-11 17:39:38.099742 q2report-0.1.29/README.md
--rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 q2report-0.1.29/PKG-INFO
+-rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2report-0.1.30/LICENSE
+-rw-r--r--   0        0        0      536 2023-07-14 11:52:23.769402 q2report-0.1.30/pyproject.toml
+-rw-r--r--   0        0        0       42 2022-12-11 17:39:38.103740 q2report-0.1.30/q2report/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:38.103740 q2report-0.1.30/q2report/q2engine/__init__.py
+-rw-r--r--   0        0        0      115 2022-12-11 17:39:38.103740 q2report-0.1.30/q2report/q2engine/q2engine_core.py
+-rw-r--r--   0        0        0       90 2022-12-11 17:39:38.107739 q2report-0.1.30/q2report/q2engine/q2engine_pyqt.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:38.107739 q2report-0.1.30/q2report/q2printer/__init__.py
+-rw-r--r--   0        0        0     8733 2023-07-12 19:54:50.695656 q2report-0.1.30/q2report/q2printer/docx_parts.py
+-rw-r--r--   0        0        0     8479 2023-06-25 22:47:50.666231 q2report-0.1.30/q2report/q2printer/q2printer.py
+-rw-r--r--   0        0        0    18818 2023-07-12 19:54:34.087531 q2report-0.1.30/q2report/q2printer/q2printer_docx.py
+-rw-r--r--   0        0        0     6126 2023-06-21 17:49:50.189551 q2report-0.1.30/q2report/q2printer/q2printer_html.py
+-rw-r--r--   0        0        0    20678 2023-06-21 17:49:55.953006 q2report-0.1.30/q2report/q2printer/q2printer_xlsx.py
+-rw-r--r--   0        0        0     8792 2023-06-21 10:36:28.504330 q2report-0.1.30/q2report/q2printer/xlsx_parts.py
+-rw-r--r--   0        0        0    30319 2023-07-13 08:40:44.679410 q2report-0.1.30/q2report/q2report.py
+-rw-r--r--   0        0        0     1708 2023-02-10 16:01:23.063515 q2report-0.1.30/q2report/q2utils.py
+-rw-r--r--   0        0        0       22 2023-07-14 11:52:30.631929 q2report-0.1.30/q2report/version.py
+-rw-r--r--   0        0        0     1486 2022-12-11 17:39:38.099742 q2report-0.1.30/README.md
+-rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 q2report-0.1.30/PKG-INFO
```

### Comparing `q2report-0.1.29/LICENSE` & `q2report-0.1.30/LICENSE`

 * *Files identical despite different names*

### Comparing `q2report-0.1.29/pyproject.toml` & `q2report-0.1.30/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "q2report"
-version = "0.1.29"
+version = "0.1.30"
 description = ""
 authors = ["Andrei Puchko <andrei.puchko@gmx.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1"
 pillow = "^9.4.0"
```

### Comparing `q2report-0.1.29/q2report/q2printer/docx_parts.py` & `q2report-0.1.30/q2report/q2printer/docx_parts.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,57 +30,56 @@
 
 """
 docx_parts[
     "image"
 ] = """
     <w:r>
     <w:drawing>
-        <wp:anchor distT="0"
+        <wp:inline distT="0"
             distB="0"
             distL="0"
             distR="0"
             simplePos="0"
             relativeHeight="2"
             behindDoc="1"
             locked="0"
             layoutInCell="1"
             allowOverlap="1"
-            
             >
             <wp:simplePos   x="0"
                             y="0"/>
             <wp:positionH relativeFrom="column">
                 <wp:align>left</wp:align>
             </wp:positionH>
             <wp:positionV relativeFrom="paragraph">
                 <wp:posOffset>0</wp:posOffset>
             </wp:positionV>
-		    <wp:extent 
+            <wp:extent
                     cx="%(width)s"
                     cy="%(height)s"/>
             <wp:effectExtent
                     l="0"
                     t="0"
                     r="0"
                     b="0"/>
             <wp:wrapNone/>
             <wp:docPr id="%(imageIndex)s"
-		          name="image%(imageIndex)s"/>
+               name="image%(imageIndex)s"/>
             <wp:cNvGraphicFramePr>
                 <a:graphicFrameLocks xmlns:a="http://schemas.openxmlformats.org/drawingml/2006/main"
                     noChangeAspect="1"/>
             </wp:cNvGraphicFramePr>
             <a:graphic xmlns:a="http://schemas.openxmlformats.org/drawingml/2006/main">
                 <a:graphicData uri="http://schemas.openxmlformats.org/drawingml/2006/picture">
                     <pic:pic xmlns:pic="http://schemas.openxmlformats.org/drawingml/2006/picture">
-					<pic:nvPicPr>
-						<pic:cNvPr id="%(imageIndex)s"
-						           name="image%(imageIndex)s.png"/>
-						<pic:cNvPicPr/>
-					</pic:nvPicPr>                    
+                    <pic:nvPicPr>
+                        <pic:cNvPr id="%(imageIndex)s"
+                                name="image%(imageIndex)s.png"/>
+                        <pic:cNvPicPr/>
+                    </pic:nvPicPr>
                         <pic:blipFill>
                             <a:blip r:embed="rId%(imageIndex)s">
                                 </a:blip>
                             <a:stretch>
                                 <a:fillRect/>
                             </a:stretch>
                         </pic:blipFill>
@@ -96,15 +95,15 @@
                             <a:prstGeom prst="rect">
                                 <a:avLst/>
                             </a:prstGeom>
                         </pic:spPr>
                     </pic:pic>
                 </a:graphicData>
             </a:graphic>
-        </wp:anchor>
+        </wp:inline>
     </w:drawing>
     </w:r>
     """
 docx_parts[
     "rels"
 ] = """<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
     <Relationships xmlns="http://schemas.openxmlformats.org/package/2006/relationships">
```

### Comparing `q2report-0.1.29/q2report/q2printer/q2printer.py` & `q2report-0.1.30/q2report/q2printer/q2printer.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.29/q2report/q2printer/q2printer_docx.py` & `q2report-0.1.30/q2report/q2printer/q2printer_docx.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,16 +176,16 @@
             </w:p>
             """
         page_param = f"""
                         <w:sectPr>
                             {header_ref_xml}
                             {footer_ref_xml}
                             <w:type w:val="nextPage"/>
-                            <w:pgSz 
-                                w:w="{self.page_width * twip_in_cm}" 
+                            <w:pgSz
+                                w:w="{self.page_width * twip_in_cm}"
                                 w:h="{self.page_height * twip_in_cm}"/>
                             <w:pgMar w:gutter="0" w:header="708" w:footer="708"
                                     w:top="{self.page_margin_top * twip_in_cm}"
                                     w:right="{self.page_margin_right * twip_in_cm}"
                                     w:bottom="{self.page_margin_bottom * twip_in_cm}"
                                     w:left="{self.page_margin_left * twip_in_cm}"
                             />
```

### Comparing `q2report-0.1.29/q2report/q2printer/q2printer_html.py` & `q2report-0.1.30/q2report/q2printer/q2printer_html.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.29/q2report/q2printer/q2printer_xlsx.py` & `q2report-0.1.30/q2report/q2printer/q2printer_xlsx.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.29/q2report/q2printer/xlsx_parts.py` & `q2report-0.1.30/q2report/q2printer/xlsx_parts.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.29/q2report/q2report.py` & `q2report-0.1.30/q2report/q2report.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,14 +161,18 @@
         footer = self._get_rows(footer)
         footer["groupby"] = groupby
         self.rows["table_groups"].append({"group_header": header, "group_footer": footer})
 
     def check_style(self, style):
         if isinstance(style, dict):
             return {x: style[x] for x in style if x in Q2Report.default_style}
+        elif isinstance(style, str):
+            if style.endswith("}") and style.startswith("{"):
+                style = style[1:-1]
+            return {x.split(":")[0]: x.split(":")[1].strip() for x in style.split(";") if ":" in x}
         else:
             return {}
 
     def extend_rows(self, row):
         while row + 1 > len(self.rows["heights"]):
             self.rows["heights"].append("0")
```

### Comparing `q2report-0.1.29/q2report/q2utils.py` & `q2report-0.1.30/q2report/q2utils.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.29/README.md` & `q2report-0.1.30/README.md`

 * *Files identical despite different names*

### Comparing `q2report-0.1.29/PKG-INFO` & `q2report-0.1.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2report
-Version: 0.1.29
+Version: 0.1.30
 Summary: 
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
 Requires-Python: >=3.8.1
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

