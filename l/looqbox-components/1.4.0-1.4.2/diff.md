# Comparing `tmp/looqbox_components-1.4.0-py3-none-any.whl.zip` & `tmp/looqbox_components-1.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,21 @@
-Zip file size: 11568 bytes, number of entries: 17
+Zip file size: 12130 bytes, number of entries: 19
 -rw-r--r--  2.0 unx      310 b- defN 23-Jul-28 17:27 looqbox_components/__init__.py
 -rw-r--r--  2.0 unx        1 b- defN 23-Jul-28 17:27 looqbox_components/templates/__init__.py
--rw-r--r--  2.0 unx     4627 b- defN 23-Jul-28 17:27 looqbox_components/templates/combo_question_link.py
+-rw-r--r--  2.0 unx     4771 b- defN 23-Aug-04 19:08 looqbox_components/templates/combo_question_link.py
 -rw-r--r--  2.0 unx     7156 b- defN 23-Jul-28 17:27 looqbox_components/templates/container.py
 -rw-r--r--  2.0 unx     2688 b- defN 23-Jul-28 17:27 looqbox_components/templates/simple_card.py
 -rw-r--r--  2.0 unx     5754 b- defN 23-Jul-28 17:27 looqbox_components/templates/tag.py
 -rw-r--r--  2.0 unx     2840 b- defN 23-Jul-28 17:27 looqbox_components/templates/toplist.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 19:08 looqbox_components/templates/resources/__init__.py
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-28 18:55 looqbox_components/templates/resources/combo_question_link.html
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-28 17:27 looqbox_components/templates/tests/__init__.py
 -rw-r--r--  2.0 unx      591 b- defN 23-Jul-28 17:27 looqbox_components/templates/tests/test_simple_card.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-28 17:27 looqbox_components/tests/__init__.py
 -rw-r--r--  2.0 unx      233 b- defN 23-Jul-28 17:27 looqbox_components/tests/test_looqbox_components.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-28 17:27 looqbox_components/utils/__init__.py
 -rw-r--r--  2.0 unx      775 b- defN 23-Jul-28 17:27 looqbox_components/utils/parent_parameters.py
--rw-r--r--  2.0 unx      989 b- defN 23-Jul-28 18:56 looqbox_components-1.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-28 18:56 looqbox_components-1.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-28 18:56 looqbox_components-1.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1613 b- defN 23-Jul-28 18:56 looqbox_components-1.4.0.dist-info/RECORD
-17 files, 27688 bytes uncompressed, 8816 bytes compressed:  68.2%
+-rw-r--r--  2.0 unx      989 b- defN 23-Aug-04 19:10 looqbox_components-1.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-04 19:10 looqbox_components-1.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Aug-04 19:10 looqbox_components-1.4.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1836 b- defN 23-Aug-04 19:10 looqbox_components-1.4.2.dist-info/RECORD
+19 files, 28165 bytes uncompressed, 9000 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -15,14 +15,20 @@
 
 Filename: looqbox_components/templates/tag.py
 Comment: 
 
 Filename: looqbox_components/templates/toplist.py
 Comment: 
 
+Filename: looqbox_components/templates/resources/__init__.py
+Comment: 
+
+Filename: looqbox_components/templates/resources/combo_question_link.html
+Comment: 
+
 Filename: looqbox_components/templates/tests/__init__.py
 Comment: 
 
 Filename: looqbox_components/templates/tests/test_simple_card.py
 Comment: 
 
 Filename: looqbox_components/tests/__init__.py
@@ -33,20 +39,20 @@
 
 Filename: looqbox_components/utils/__init__.py
 Comment: 
 
 Filename: looqbox_components/utils/parent_parameters.py
 Comment: 
 
-Filename: looqbox_components-1.4.0.dist-info/METADATA
+Filename: looqbox_components-1.4.2.dist-info/METADATA
 Comment: 
 
-Filename: looqbox_components-1.4.0.dist-info/WHEEL
+Filename: looqbox_components-1.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: looqbox_components-1.4.0.dist-info/top_level.txt
+Filename: looqbox_components-1.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: looqbox_components-1.4.0.dist-info/RECORD
+Filename: looqbox_components-1.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## looqbox_components/templates/combo_question_link.py

```diff
@@ -44,55 +44,58 @@
             show_preview: bool = True,
             clear_button_text: str = "Limpar Filtros"
     ):
         super().__init__()
         self.base_question = base_question
         self.show_preview = str(show_preview).lower()
         self.clear_button_text = clear_button_text
-        self._selects: List[Dict] = []
+        self._selects_lists: List[Dict] = []
 
-    def add_combo_filter(self, box_tile: str, is_multiselect: bool, option_header: str,box_content: dict):
-        self._selects.append({"box_name": box_tile, "is_multiselect": is_multiselect,
-                              "value": option_header, "content": box_content})
+    def add_combo_filter(self, box_tile: str, is_multiselect: bool, option_header: str, box_content: dict):
+        self._selects_lists.append({"box_name": box_tile, "is_multiselect": is_multiselect,
+                                    "value": option_header, "content": box_content})
 
-    def _build_option(self, options, value):
-        raw_options = [(f"{{label: '{option.get('label')}', value: '{value} {option.get('label')}'"
-                        f"{self._build_filter_condition_statement(option.get('filter'))} }}") for option in options]
+    def _build_options_list(self, options_content, value):
+        options = [(f"{{label: '{option.get('label')}', value: '{value} {option.get('label')}'"
+                    f"{self._build_filter_condition_statement(option.get('filter'))} }}") for option in options_content]
 
-        combo_options = [", ".join(option for option in raw_options)]
-        return combo_options[0]
+        formated_combo_options = [", ".join(option for option in options)]
+        return formated_combo_options[0]
 
-    def _build_filter_condition_statement(self, filter: None|str) -> str:
+    def _build_filter_condition_statement(self, filter: None | str) -> str:
         base_filter = ", filter: '"
 
         return "" if filter is None else base_filter + filter + "'"
 
     def _build_select(self, select):
-        options = self._build_option(select.get("content"), select.get("value", ""))
-        select_html = ("{name: '" + select.get("box_name", "")  + "', multiSelect: " +
-                       str(select.get("is_multiselect", "false")).lower() + ", options: [" + options + "]}")
-        return select_html
-
-    def _build(self):
-        selects = ", ".join([self._build_select(select) for select in self._selects])
-
-        combo_question_link = self._get_combo_question_link_html_template().format(self.base_question,
-                                                                                   self.show_preview,
-                                                                                   self.clear_button_text,
-                                                                                   selects)
-    
+        options = self._build_options_list(select.get("content"), select.get("value", ""))
+        select_box_html = ("{name: '" + select.get("box_name", "") + "', multiSelect: " +
+                           str(select.get("is_multiselect", "false")).lower() + ", options: [" + options + "]}")
+        return select_box_html
+
+    def _build_component_html(self):
+        selects = ", ".join([self._build_select(select) for select in self._selects_lists])
+
+        combo_question_link = self._enrich_base_template(selects)
+
         return ObjHTML(combo_question_link)
 
+    def _enrich_base_template(self, selects):
+        return self._get_combo_question_link_html_template().format(self.base_question,
+                                                                    self.show_preview,
+                                                                    self.clear_button_text,
+                                                                    selects)
+
     def _get_combo_question_link_html_template(self) -> str:
         import os
-        html_template_path = os.path.join(os.path.dirname(__file__),"resources", "combo_question_link.html")
+        html_template_path = os.path.join(os.path.dirname(__file__), "resources", "combo_question_link.html")
         try:
             with open(html_template_path, "r") as template_file:
                 combo_question_link_template = "".join(template_file.readlines())
                 template_file.close()
             return combo_question_link_template
         except IOError as error:
             raise error
-        
+
     def to_json_structure(self, visitor: BaseRender):
-        self.combobox = self._build()
+        self.combobox = self._build_component_html()
         return self.combobox.to_json_structure(visitor)
```

## Comparing `looqbox_components-1.4.0.dist-info/METADATA` & `looqbox_components-1.4.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: looqbox-components
-Version: 1.4.0
+Version: 1.4.2
 Summary: A looqbox package with most used visual components templates
 Home-page: https://github.com/looqbox/python-visual-components
 Author: Looqbox
 Author-email: admin@looqbox.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `looqbox_components-1.4.0.dist-info/RECORD` & `looqbox_components-1.4.2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 looqbox_components/__init__.py,sha256=KMMRTGihM-5sVtBrhFtan6um6C_iyl2XIWwpAMelkAg,310
 looqbox_components/templates/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-looqbox_components/templates/combo_question_link.py,sha256=5g4j_PSKLto-lHOL0BK7GqoAJ6QirmJed2tkZbFqcuo,4627
+looqbox_components/templates/combo_question_link.py,sha256=Cg8b3rEVe6TWCCoiFDpM8-w2OY9DY2aRdEqxxjAUAuQ,4771
 looqbox_components/templates/container.py,sha256=QFClUUkX2GtwiT8MmIPJQmSrfZBg3PRnWM01BQodMfw,7156
 looqbox_components/templates/simple_card.py,sha256=_OEaulW5bI_D9nUy3nEHErS2YXeReFJAROCOtJBkTDo,2688
 looqbox_components/templates/tag.py,sha256=qqUpb2Tn86kjgSn1kZNccM7BlaLbtZqHs40NhW9UDrg,5754
 looqbox_components/templates/toplist.py,sha256=mAlFkUBYXMMqSSIz5MogMascE1OfzVoT5sfGfFiuC5Y,2840
+looqbox_components/templates/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+looqbox_components/templates/resources/combo_question_link.html,sha256=K6LMpt9de8jX6vRxZwBDYWK0p8cKDt59HeoUgPLHPXc,110
 looqbox_components/templates/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 looqbox_components/templates/tests/test_simple_card.py,sha256=p7axi8j3Fqs5Ka_GSSDM7JImPZaH-xpDc4ZmBYCdupU,591
 looqbox_components/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 looqbox_components/tests/test_looqbox_components.py,sha256=8fVRfEvqcxlJDuNp6RlucKwH13JMCrXkeGgSmkdxonU,233
 looqbox_components/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 looqbox_components/utils/parent_parameters.py,sha256=SEgVvejN3PqjcSkKJztrYykjo-m626BY0s1WvpGEmOs,775
-looqbox_components-1.4.0.dist-info/METADATA,sha256=d3vyo9R9HEEJVGmEuyO9DmE83wRwdhDelfzi6Vr-lM4,989
-looqbox_components-1.4.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-looqbox_components-1.4.0.dist-info/top_level.txt,sha256=Zb_QlF8DlA-rP1wb-5-vbk_U_exlVnC4IXl1bBro5kQ,19
-looqbox_components-1.4.0.dist-info/RECORD,,
+looqbox_components-1.4.2.dist-info/METADATA,sha256=eDjexVsUZwtb3438-Ujtk5eLfxHb8fVJzCGwHC9IoVs,989
+looqbox_components-1.4.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+looqbox_components-1.4.2.dist-info/top_level.txt,sha256=Zb_QlF8DlA-rP1wb-5-vbk_U_exlVnC4IXl1bBro5kQ,19
+looqbox_components-1.4.2.dist-info/RECORD,,
```

