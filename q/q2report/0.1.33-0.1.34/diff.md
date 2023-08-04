# Comparing `tmp/q2report-0.1.33.tar.gz` & `tmp/q2report-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2report-0.1.33.tar", max compression
+gzip compressed data, was "q2report-0.1.34.tar", max compression
```

## Comparing `q2report-0.1.33.tar` & `q2report-0.1.34.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2report-0.1.33/LICENSE
--rw-r--r--   0        0        0      537 2023-07-26 23:24:03.605825 q2report-0.1.33/pyproject.toml
--rw-r--r--   0        0        0       42 2022-12-11 17:39:38.103740 q2report-0.1.33/q2report/__init__.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:38.103740 q2report-0.1.33/q2report/q2engine/__init__.py
--rw-r--r--   0        0        0      115 2022-12-11 17:39:38.103740 q2report-0.1.33/q2report/q2engine/q2engine_core.py
--rw-r--r--   0        0        0       90 2022-12-11 17:39:38.107739 q2report-0.1.33/q2report/q2engine/q2engine_pyqt.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:38.107739 q2report-0.1.33/q2report/q2printer/__init__.py
--rw-r--r--   0        0        0     8733 2023-07-12 19:54:50.695656 q2report-0.1.33/q2report/q2printer/docx_parts.py
--rw-r--r--   0        0        0     8338 2023-07-26 08:18:01.892779 q2report-0.1.33/q2report/q2printer/q2printer.py
--rw-r--r--   0        0        0    18675 2023-07-26 08:17:38.485026 q2report-0.1.33/q2report/q2printer/q2printer_docx.py
--rw-r--r--   0        0        0     5983 2023-07-26 08:17:46.036036 q2report-0.1.33/q2report/q2printer/q2printer_html.py
--rw-r--r--   0        0        0    20534 2023-07-26 08:17:54.125833 q2report-0.1.33/q2report/q2printer/q2printer_xlsx.py
--rw-r--r--   0        0        0     8792 2023-06-21 10:36:28.504330 q2report-0.1.33/q2report/q2printer/xlsx_parts.py
--rw-r--r--   0        0        0    30897 2023-07-26 08:17:30.792654 q2report-0.1.33/q2report/q2report.py
--rw-r--r--   0        0        0     1708 2023-02-10 16:01:23.063515 q2report-0.1.33/q2report/q2utils.py
--rw-r--r--   0        0        0       22 2023-07-26 23:24:05.374565 q2report-0.1.33/q2report/version.py
--rw-r--r--   0        0        0     1486 2022-12-11 17:39:38.099742 q2report-0.1.33/README.md
--rw-r--r--   0        0        0     1862 1970-01-01 00:00:00.000000 q2report-0.1.33/PKG-INFO
+-rw-r--r--   0        0        0    10347 2023-08-04 11:01:45.872644 q2report-0.1.34/LICENSE
+-rw-r--r--   0        0        0      537 2023-08-04 12:07:41.436086 q2report-0.1.34/pyproject.toml
+-rw-r--r--   0        0        0       42 2022-12-11 17:39:38.103740 q2report-0.1.34/q2report/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:38.103740 q2report-0.1.34/q2report/q2engine/__init__.py
+-rw-r--r--   0        0        0      115 2022-12-11 17:39:38.103740 q2report-0.1.34/q2report/q2engine/q2engine_core.py
+-rw-r--r--   0        0        0       90 2022-12-11 17:39:38.107739 q2report-0.1.34/q2report/q2engine/q2engine_pyqt.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:38.107739 q2report-0.1.34/q2report/q2printer/__init__.py
+-rw-r--r--   0        0        0     8044 2023-08-04 11:23:35.242782 q2report-0.1.34/q2report/q2printer/docx_parts.py
+-rw-r--r--   0        0        0     8338 2023-08-04 11:01:45.883638 q2report-0.1.34/q2report/q2printer/q2printer.py
+-rw-r--r--   0        0        0    18673 2023-08-04 11:01:45.885650 q2report-0.1.34/q2report/q2printer/q2printer_docx.py
+-rw-r--r--   0        0        0     5983 2023-08-04 11:01:45.885650 q2report-0.1.34/q2report/q2printer/q2printer_html.py
+-rw-r--r--   0        0        0    20534 2023-08-04 11:01:45.886650 q2report-0.1.34/q2report/q2printer/q2printer_xlsx.py
+-rw-r--r--   0        0        0     8779 2023-08-04 11:52:45.531773 q2report-0.1.34/q2report/q2printer/xlsx_parts.py
+-rw-r--r--   0        0        0    30897 2023-08-04 11:01:45.889647 q2report-0.1.34/q2report/q2report.py
+-rw-r--r--   0        0        0     1708 2023-02-10 16:01:23.063515 q2report-0.1.34/q2report/q2utils.py
+-rw-r--r--   0        0        0       22 2023-08-04 12:07:43.086144 q2report-0.1.34/q2report/version.py
+-rw-r--r--   0        0        0     1486 2022-12-11 17:39:38.099742 q2report-0.1.34/README.md
+-rw-r--r--   0        0        0     1862 1970-01-01 00:00:00.000000 q2report-0.1.34/PKG-INFO
```

### Comparing `q2report-0.1.33/LICENSE` & `q2report-0.1.34/LICENSE`

 * *Files identical despite different names*

### Comparing `q2report-0.1.33/pyproject.toml` & `q2report-0.1.34/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "q2report"
-version = "0.1.33"
+version = "0.1.34"
 description = ""
 authors = ["Andrei Puchko <andrei.puchko@gmx.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1"
 pillow = ">=9.4.0"
```

### Comparing `q2report-0.1.33/q2report/q2printer/docx_parts.py` & `q2report-0.1.34/q2report/q2printer/docx_parts.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,61 +25,36 @@
     xmlns:m="http://schemas.openxmlformats.org/officeDocument/2006/math"
     xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships"
     xmlns:o="urn:schemas-microsoft-com:office:office"
     xmlns:ve="http://schemas.openxmlformats.org/markup-compatibility/2006">
 <w:body>
 
 """
+
 docx_parts[
     "image"
 ] = """
     <w:r>
     <w:drawing>
-        <wp:inline distT="0"
-            distB="0"
-            distL="0"
-            distR="0"
-            simplePos="0"
-            relativeHeight="2"
-            behindDoc="1"
-            locked="0"
-            layoutInCell="1"
-            allowOverlap="1"
-            >
-            <wp:simplePos   x="0"
-                            y="0"/>
-            <wp:positionH relativeFrom="column">
-                <wp:align>left</wp:align>
-            </wp:positionH>
-            <wp:positionV relativeFrom="paragraph">
-                <wp:posOffset>0</wp:posOffset>
-            </wp:positionV>
-            <wp:extent
-                    cx="%(width)s"
-                    cy="%(height)s"/>
-            <wp:effectExtent
-                    l="0"
-                    t="0"
-                    r="0"
-                    b="0"/>
-            <wp:wrapNone/>
-            <wp:docPr id="%(imageIndex)s"
-               name="image%(imageIndex)s"/>
+        <wp:inline distT="0" distB="0" distL="0" distR="0">
+            <wp:extent cx="%(width)s" cy="%(height)s"/>
+            <wp:effectExtent l="0" t="0" r="0" b="0"/>
+            <wp:docPr id="%(imageIndex)s" name="image%(imageIndex)s"/>
             <wp:cNvGraphicFramePr>
                 <a:graphicFrameLocks xmlns:a="http://schemas.openxmlformats.org/drawingml/2006/main"
                     noChangeAspect="1"/>
             </wp:cNvGraphicFramePr>
             <a:graphic xmlns:a="http://schemas.openxmlformats.org/drawingml/2006/main">
                 <a:graphicData uri="http://schemas.openxmlformats.org/drawingml/2006/picture">
                     <pic:pic xmlns:pic="http://schemas.openxmlformats.org/drawingml/2006/picture">
-                    <pic:nvPicPr>
+                        <pic:nvPicPr>
                         <pic:cNvPr id="%(imageIndex)s"
                                 name="image%(imageIndex)s.png"/>
                         <pic:cNvPicPr/>
-                    </pic:nvPicPr>
+                    </pic:nvPicPr>                    
                         <pic:blipFill>
                             <a:blip r:embed="rId%(imageIndex)s">
                                 </a:blip>
                             <a:stretch>
                                 <a:fillRect/>
                             </a:stretch>
                         </pic:blipFill>
@@ -99,14 +74,15 @@
                     </pic:pic>
                 </a:graphicData>
             </a:graphic>
         </wp:inline>
     </w:drawing>
     </w:r>
     """
+
 docx_parts[
     "rels"
 ] = """<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
     <Relationships xmlns="http://schemas.openxmlformats.org/package/2006/relationships">
     <Relationship Id="rId1"
         Type="http://schemas.openxmlformats.org/officeDocument/2006/relationships/officeDocument"
         Target="word/document.xml"/>
```

### Comparing `q2report-0.1.33/q2report/q2printer/q2printer.py` & `q2report-0.1.34/q2report/q2printer/q2printer.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.33/q2report/q2printer/q2printer_docx.py` & `q2report-0.1.34/q2report/q2printer/q2printer_docx.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,14 @@
 
     def add_table_cell(self, cell_style, cell_text, cell_width, merge_str, images=[]):
         borders = self.get_cell_borders(cell_style)
         margins = self.get_cell_paddings(cell_style)
         para_params = self.get_paragraph_params(cell_style)
         para_text = self.get_paragraph_text(cell_style, cell_text, para_params)
         valign = self.get_vertical_align(cell_style)
-
         # self.document.append(
         return f"""
                 <w:tc>
                     <w:tcPr>
                         <w:tcW w:w="{int(cell_width * twip_in_cm)}" w:type="dxa"/>
                         {valign}
                         {merge_str}
```

### Comparing `q2report-0.1.33/q2report/q2printer/q2printer_html.py` & `q2report-0.1.34/q2report/q2printer/q2printer_html.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.33/q2report/q2printer/q2printer_xlsx.py` & `q2report-0.1.34/q2report/q2printer/q2printer_xlsx.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.33/q2report/q2printer/xlsx_parts.py` & `q2report-0.1.34/q2report/q2printer/xlsx_parts.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,19 @@
             <xdr:row>%(_row)s</xdr:row>
             <xdr:rowOff>0</xdr:rowOff>
         </xdr:from>
         <xdr:ext
             cx="%(_width)s"
             cy="%(_height)s"/>
         <xdr:pic>
-			<xdr:nvPicPr>
+            <xdr:nvPicPr>
                 <xdr:cNvPr id="%(_id)s"
                         name="image%(_id)s"/>
                 <xdr:cNvPicPr>
-                    <a:picLocks noChangeAspect="1"/>
+                    <a:picLocks/>
                 </xdr:cNvPicPr>
             </xdr:nvPicPr>
             <xdr:blipFill>
                 <a:blip xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships"
                         r:embed="rId%(_id)s">
                 </a:blip>
                 <a:stretch>
@@ -50,21 +50,21 @@
                 </a:xfrm>
                 <a:prstGeom prst="rect">
                     <a:avLst/>
                 </a:prstGeom>
             </xdr:spPr>
         </xdr:pic>
         <xdr:clientData/>
- </xdr:oneCellAnchor>"""
+</xdr:oneCellAnchor>"""
 
 
 xlsx_parts[
     "xl/drawings/drawing.xml"
 ] = """<xdr:wsDr xmlns:xdr="http://schemas.openxmlformats.org/drawingml/2006/spreadsheetDrawing"
-          xmlns:a="http://schemas.openxmlformats.org/drawingml/2006/main">
+        xmlns:a="http://schemas.openxmlformats.org/drawingml/2006/main">
             %s
     </xdr:wsDr>"""
 xlsx_parts[
     "xl/drawings/_rels/drawing.xml.rels"
 ] = """<?xml version="1.0" encoding="UTF-8"?>
     <Relationships xmlns="http://schemas.openxmlformats.org/package/2006/relationships">
         %s
```

### Comparing `q2report-0.1.33/q2report/q2report.py` & `q2report-0.1.34/q2report/q2report.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.33/q2report/q2utils.py` & `q2report-0.1.34/q2report/q2utils.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.33/README.md` & `q2report-0.1.34/README.md`

 * *Files identical despite different names*

### Comparing `q2report-0.1.33/PKG-INFO` & `q2report-0.1.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2report
-Version: 0.1.33
+Version: 0.1.34
 Summary: 
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
 Requires-Python: >=3.8.1
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

