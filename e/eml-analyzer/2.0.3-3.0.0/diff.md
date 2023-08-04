# Comparing `tmp/eml-analyzer-2.0.3.tar.gz` & `tmp/eml-analyzer-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Florian\Documents\gits\eml_analyzer\dist\.tmp-3snd_e3m\eml-analyzer-2.0.3.tar", last modified: Thu Apr  6 21:47:51 2023, max compression
+gzip compressed data, was "eml-analyzer-3.0.0.tar", last modified: Fri Aug  4 18:51:31 2023, max compression
```

## Comparing `eml-analyzer-2.0.3.tar` & `eml-analyzer-3.0.0.tar`

### file list

```diff
@@ -1,42 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 21:47:51.195160 eml-analyzer-2.0.3/
--rw-rw-rw-   0        0        0     1090 2021-01-25 20:55:07.000000 eml-analyzer-2.0.3/LICENSE
--rw-rw-rw-   0        0        0     5692 2023-04-06 21:47:51.195160 eml-analyzer-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5356 2023-02-27 09:16:45.000000 eml-analyzer-2.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 21:47:51.172588 eml-analyzer-2.0.3/eml_analyzer/
--rw-rw-rw-   0        0        0        0 2021-01-25 20:55:07.000000 eml-analyzer-2.0.3/eml_analyzer/__init__.py
--rw-rw-rw-   0        0        0     8118 2023-01-21 10:13:47.000000 eml-analyzer-2.0.3/eml_analyzer/cli_script.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:47:51.180817 eml-analyzer-2.0.3/eml_analyzer/library/
--rw-rw-rw-   0        0        0        0 2022-12-31 02:00:50.000000 eml-analyzer-2.0.3/eml_analyzer/library/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:47:51.183885 eml-analyzer-2.0.3/eml_analyzer/library/outputs/
--rw-rw-rw-   0        0        0      127 2022-12-31 02:00:50.000000 eml-analyzer-2.0.3/eml_analyzer/library/outputs/__init__.py
--rw-rw-rw-   0        0        0     1461 2022-12-31 02:00:50.000000 eml-analyzer-2.0.3/eml_analyzer/library/outputs/abstract_output.py
--rw-rw-rw-   0        0        0     4549 2023-01-21 10:15:27.000000 eml-analyzer-2.0.3/eml_analyzer/library/outputs/json_output.py
--rw-rw-rw-   0        0        0     5145 2023-01-21 10:13:47.000000 eml-analyzer-2.0.3/eml_analyzer/library/outputs/standard_output.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:47:51.187950 eml-analyzer-2.0.3/eml_analyzer/library/parser/
--rw-rw-rw-   0        0        0      165 2022-12-31 02:00:50.000000 eml-analyzer-2.0.3/eml_analyzer/library/parser/__init__.py
--rw-rw-rw-   0        0        0      657 2022-12-31 02:00:50.000000 eml-analyzer-2.0.3/eml_analyzer/library/parser/attachment.py
--rw-rw-rw-   0        0        0    10063 2023-04-06 21:40:31.000000 eml-analyzer-2.0.3/eml_analyzer/library/parser/parsed_email.py
--rw-rw-rw-   0        0        0     1245 2023-02-27 08:57:25.000000 eml-analyzer-2.0.3/eml_analyzer/library/parser/printable_filename.py
--rw-rw-rw-   0        0        0      614 2022-12-31 02:00:50.000000 eml-analyzer-2.0.3/eml_analyzer/library/parser/structure_item.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:47:51.179782 eml-analyzer-2.0.3/eml_analyzer.egg-info/
--rw-rw-rw-   0        0        0     5692 2023-04-06 21:47:51.000000 eml-analyzer-2.0.3/eml_analyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1059 2023-04-06 21:47:51.000000 eml-analyzer-2.0.3/eml_analyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 21:47:51.000000 eml-analyzer-2.0.3/eml_analyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-06 21:47:51.000000 eml-analyzer-2.0.3/eml_analyzer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-04-06 21:47:51.000000 eml-analyzer-2.0.3/eml_analyzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-06 21:47:51.000000 eml-analyzer-2.0.3/eml_analyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 21:47:51.196174 eml-analyzer-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1102 2023-04-06 21:45:13.000000 eml-analyzer-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:47:51.187950 eml-analyzer-2.0.3/tests/
--rw-rw-rw-   0        0        0        0 2022-12-31 02:00:50.000000 eml-analyzer-2.0.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:47:51.188971 eml-analyzer-2.0.3/tests/library/
--rw-rw-rw-   0        0        0        0 2022-12-31 02:00:50.000000 eml-analyzer-2.0.3/tests/library/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:47:51.189978 eml-analyzer-2.0.3/tests/library/outputs/
--rw-rw-rw-   0        0        0        0 2022-12-31 02:00:50.000000 eml-analyzer-2.0.3/tests/library/outputs/__init__.py
--rw-rw-rw-   0        0        0     8120 2023-01-21 10:15:27.000000 eml-analyzer-2.0.3/tests/library/outputs/test_json_output.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:47:51.194145 eml-analyzer-2.0.3/tests/library/parser/
--rw-rw-rw-   0        0        0        0 2022-12-31 02:00:50.000000 eml-analyzer-2.0.3/tests/library/parser/__init__.py
--rw-rw-rw-   0        0        0     1117 2023-02-27 08:57:25.000000 eml-analyzer-2.0.3/tests/library/parser/test_attachment.py
--rw-rw-rw-   0        0        0    19641 2023-04-06 21:35:43.000000 eml-analyzer-2.0.3/tests/library/parser/test_parsed_email.py
--rw-rw-rw-   0        0        0     1938 2023-02-27 08:57:25.000000 eml-analyzer-2.0.3/tests/library/parser/test_printable_filename.py
--rw-rw-rw-   0        0        0     1536 2022-12-31 02:00:50.000000 eml-analyzer-2.0.3/tests/library/parser/test_structure_item.py
+drwxrwxrwx   0        0        0        0 2023-08-04 18:51:31.459250 eml-analyzer-3.0.0/
+-rw-rw-rw-   0        0        0     1090 2023-08-04 13:55:38.000000 eml-analyzer-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0     5692 2023-08-04 18:51:31.459250 eml-analyzer-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5356 2023-08-04 13:55:38.000000 eml-analyzer-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 18:51:31.444953 eml-analyzer-3.0.0/eml_analyzer/
+-rw-rw-rw-   0        0        0        0 2023-08-04 13:55:38.000000 eml-analyzer-3.0.0/eml_analyzer/__init__.py
+-rw-rw-rw-   0        0        0     8136 2023-08-04 18:50:14.000000 eml-analyzer-3.0.0/eml_analyzer/cli_script.py
+drwxrwxrwx   0        0        0        0 2023-08-04 18:51:31.451145 eml-analyzer-3.0.0/eml_analyzer/library/
+-rw-rw-rw-   0        0        0        0 2023-08-04 13:55:38.000000 eml-analyzer-3.0.0/eml_analyzer/library/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 18:51:31.454175 eml-analyzer-3.0.0/eml_analyzer/library/outputs/
+-rw-rw-rw-   0        0        0      127 2023-08-04 13:55:38.000000 eml-analyzer-3.0.0/eml_analyzer/library/outputs/__init__.py
+-rw-rw-rw-   0        0        0     1461 2023-08-04 13:55:38.000000 eml-analyzer-3.0.0/eml_analyzer/library/outputs/abstract_output.py
+-rw-rw-rw-   0        0        0     4549 2023-08-04 13:55:38.000000 eml-analyzer-3.0.0/eml_analyzer/library/outputs/json_output.py
+-rw-rw-rw-   0        0        0     5145 2023-08-04 13:55:38.000000 eml-analyzer-3.0.0/eml_analyzer/library/outputs/standard_output.py
+drwxrwxrwx   0        0        0        0 2023-08-04 18:51:31.458735 eml-analyzer-3.0.0/eml_analyzer/library/parser/
+-rw-rw-rw-   0        0        0      165 2023-08-04 13:55:38.000000 eml-analyzer-3.0.0/eml_analyzer/library/parser/__init__.py
+-rw-rw-rw-   0        0        0      657 2023-08-04 13:55:38.000000 eml-analyzer-3.0.0/eml_analyzer/library/parser/attachment.py
+-rw-rw-rw-   0        0        0    11389 2023-08-04 18:50:14.000000 eml-analyzer-3.0.0/eml_analyzer/library/parser/parsed_email.py
+-rw-rw-rw-   0        0        0     2065 2023-08-04 18:50:14.000000 eml-analyzer-3.0.0/eml_analyzer/library/parser/printable_filename.py
+-rw-rw-rw-   0        0        0      614 2023-08-04 13:55:38.000000 eml-analyzer-3.0.0/eml_analyzer/library/parser/structure_item.py
+drwxrwxrwx   0        0        0        0 2023-08-04 18:51:31.450133 eml-analyzer-3.0.0/eml_analyzer.egg-info/
+-rw-rw-rw-   0        0        0     5692 2023-08-04 18:51:31.000000 eml-analyzer-3.0.0/eml_analyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      732 2023-08-04 18:51:31.000000 eml-analyzer-3.0.0/eml_analyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 18:51:31.000000 eml-analyzer-3.0.0/eml_analyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-08-04 18:51:31.000000 eml-analyzer-3.0.0/eml_analyzer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-08-04 18:51:31.000000 eml-analyzer-3.0.0/eml_analyzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-04 18:51:31.000000 eml-analyzer-3.0.0/eml_analyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 18:51:31.459250 eml-analyzer-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1102 2023-08-04 18:50:14.000000 eml-analyzer-3.0.0/setup.py
```

### Comparing `eml-analyzer-2.0.3/LICENSE` & `eml-analyzer-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eml-analyzer-2.0.3/PKG-INFO` & `eml-analyzer-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eml-analyzer
-Version: 2.0.3
+Version: 3.0.0
 Summary: A cli script to analyze an E-Mail in the eml format for viewing the header, extracting attachments, etc.
 Home-page: https://github.com/wahlflo/eml_analyzer
 Author: Florian Wahl
 Author-email: florian.wahl.developer@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eml-analyzer-2.0.3/README.md` & `eml-analyzer-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `eml-analyzer-2.0.3/eml_analyzer/cli_script.py` & `eml-analyzer-3.0.0/eml_analyzer/cli_script.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from eml_analyzer.library.outputs import AbstractOutput, StandardOutput, JsonOutput
 from eml_analyzer.library.parser import ParsedEmail, EmlParsingException, Attachment
 
 
 def main():
     argument_parser = argparse.ArgumentParser(prog='emlAnalyzer', description='A CLI script to analyze an email in the EML format for viewing headers, extracting attachments, etc.')
-    argument_parser.add_argument('-i', '--input', help="Path to the EML file. Accepts standard input if omitted", type=argparse.FileType('r'), nargs='?', default=sys.stdin)
+    argument_parser.add_argument('-i', '--input', help="Path to the EML file. Accepts standard input if omitted", type=argparse.FileType('r', encoding='utf-8'), nargs='?', default=sys.stdin)
     argument_parser.add_argument('--header', action='store_true', default=False, help="Shows the headers")
     argument_parser.add_argument('-x', '--tracking', action='store_true', default=False, help="Shows content which is reloaded from external resources in the HTML part")
     argument_parser.add_argument('-a', '--attachments', action='store_true', default=False, help="Lists attachments")
     argument_parser.add_argument('--text', action='store_true', default=False, help="Shows plaintext")
     argument_parser.add_argument('--html', action='store_true', default=False, help="Shows HTML")
     argument_parser.add_argument('-s', '--structure', action='store_true', default=False, help="Shows structure of the E-Mail")
     argument_parser.add_argument('-u', '--url', action='store_true', default=False, help="Shows embedded clickable links and urls in the HTML and text part")
```

### Comparing `eml-analyzer-2.0.3/eml_analyzer/library/outputs/abstract_output.py` & `eml-analyzer-3.0.0/eml_analyzer/library/outputs/abstract_output.py`

 * *Files identical despite different names*

### Comparing `eml-analyzer-2.0.3/eml_analyzer/library/outputs/json_output.py` & `eml-analyzer-3.0.0/eml_analyzer/library/outputs/json_output.py`

 * *Files identical despite different names*

### Comparing `eml-analyzer-2.0.3/eml_analyzer/library/outputs/standard_output.py` & `eml-analyzer-3.0.0/eml_analyzer/library/outputs/standard_output.py`

 * *Files identical despite different names*

### Comparing `eml-analyzer-2.0.3/eml_analyzer/library/parser/attachment.py` & `eml-analyzer-3.0.0/eml_analyzer/library/parser/attachment.py`

 * *Files identical despite different names*

### Comparing `eml-analyzer-2.0.3/eml_analyzer/library/parser/parsed_email.py` & `eml-analyzer-3.0.0/eml_analyzer/library/parser/parsed_email.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import email.message
 import urllib.parse
 import html
 import warnings
 from typing import NamedTuple, List, Tuple, Set
 
 from eml_analyzer.library.parser.attachment import Attachment
+from eml_analyzer.library.parser.printable_filename import decode_ASCII_encoded_string
 from eml_analyzer.library.parser.structure_item import StructureItem
 
 
 class EmlParsingException(Exception):
     pass
 
 
@@ -44,15 +45,15 @@
         return self._error_messages
 
     def _add_error_messages(self, error_message: str) -> None:
         self._error_messages.append(error_message)
 
     def get_header(self) -> List[Tuple[str, any]]:
         """ returns list of key-value pairs of header entries """
-        return self._parsed_email.items()
+        return [(key, decode_ASCII_encoded_string(value)) for key, value in self._parsed_email.items()]
 
     def get_structure(self) -> StructureItem:
         return StructureItem(message=self._parsed_email)
 
     def get_text_content(self) -> str or None:
         return self._get_decoded_payload_with_first_matching_type(content_type='text/plain')
 
@@ -82,47 +83,73 @@
                 found_payload = ParsedEmail._get_first_email_payload_with_matching_type(message=child_payload, content_type=content_type)
                 if found_payload is not None:
                     return found_payload
         return None
 
     @staticmethod
     def _get_decoded_payload_from_message(message: email.message.Message) -> None or str:
+        transfer_encoding = ParsedEmail._header_lookup_first_element(message=message, key='content-transfer-encoding')
+        if transfer_encoding in {'7bit', '8bit', 'binary'}:
+            return message.get_payload(decode=False)
+
         payload_in_bytes = message.get_payload(decode=True)
 
         list_of_possible_encodings = ParsedEmail._create_list_of_possible_encodings(message=message)
 
         for encoding_format in list_of_possible_encodings:
             try:
                 return payload_in_bytes.decode(encoding_format)
-            except ValueError:
+            except ValueError as error:
+                print('Error: ' + str(error))
                 continue
         raise PayloadDecodingException('Payload could not be decoded')
 
     @staticmethod
     def _create_list_of_possible_encodings(message: email.message.Message) -> list:
         """ creates a list of the most possible encodings of a payload """
         list_of_possible_encodings = list()
 
+        header_values = ParsedEmail._header_lookup(message=message, key='content-type')
+
         # at first add the encodings mentioned in the object header
-        for k, v in message.items():
-            k = str(k).lower()
-            v = str(v).lower()
-            if k == 'content-type':
-                entries = v.split(';')
-                for entry in entries:
-                    entry = entry.strip()
-                    if entry.startswith('charset='):
-                        encoding = entry.replace('charset=', '').replace('"', '')
-                        list_of_possible_encodings.append(encoding)
+        for v in header_values:
+            entries = v.split(';')
+            for entry in entries:
+                entry = entry.strip()
+                if entry.startswith('charset='):
+                    encoding = entry.replace('charset=', '').replace('"', '')
+                    list_of_possible_encodings.append(encoding)
 
         for x in ['utf-8', 'windows-1251', 'iso-8859-1', 'us-ascii', 'iso-8859-15']:
             if x not in list_of_possible_encodings:
                 list_of_possible_encodings.append(x)
         return list_of_possible_encodings
 
+    @staticmethod
+    def _payload_needs_decoding(message: email.message.Message) -> bool:
+        transfer_encoding = ParsedEmail._header_lookup_first_element(message=message, key='content-transfer-encoding')
+        if transfer_encoding is None:
+            return True
+        return transfer_encoding not in {'7bit', '8bit', 'binary'}
+
+    @staticmethod
+    def _header_lookup_first_element(message: email.message.Message, key: str) -> str or None:
+        for header_key, value in message.items():
+            if str(header_key).lower() == key:
+                return str(value).lower()
+        return None
+
+    @staticmethod
+    def _header_lookup(message: email.message.Message, key: str) -> [str]:
+        values = list()
+        for header_key, value in message.items():
+            if str(header_key).lower() == key:
+                values.append(str(value).lower())
+        return values
+
     def get_attachments(self) -> List[Attachment]:
         return_list = list()
         counter = 0
         for child in self._parsed_email.walk():
             if child.get_filename() is not None:
                 counter += 1
                 return_list.append(Attachment(message=child, index=counter))
```

### Comparing `eml-analyzer-2.0.3/eml_analyzer/library/parser/structure_item.py` & `eml-analyzer-3.0.0/eml_analyzer/library/parser/structure_item.py`

 * *Files identical despite different names*

### Comparing `eml-analyzer-2.0.3/eml_analyzer.egg-info/PKG-INFO` & `eml-analyzer-3.0.0/eml_analyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eml-analyzer
-Version: 2.0.3
+Version: 3.0.0
 Summary: A cli script to analyze an E-Mail in the eml format for viewing the header, extracting attachments, etc.
 Home-page: https://github.com/wahlflo/eml_analyzer
 Author: Florian Wahl
 Author-email: florian.wahl.developer@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eml-analyzer-2.0.3/setup.py` & `eml-analyzer-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = readme_file.read()
     # remove badges in Readme
     long_description = '# emlAnalyzer' + long_description.split('# emlAnalyzer')[1]
 
 
 setuptools.setup(
     name="eml-analyzer",
-    version="2.0.3",
+    version="3.0.0",
     author="Florian Wahl",
     author_email="florian.wahl.developer@gmail.com",
     description="A cli script to analyze an E-Mail in the eml format for viewing the header, extracting attachments, etc.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wahlflo/eml_analyzer",
     packages=setuptools.find_packages(exclude=("tests", "tests.*")),
```

