# Comparing `tmp/ptcrossd-1.0.1.tar.gz` & `tmp/ptcrossd-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptcrossd-1.0.1.tar", last modified: Mon Jul 31 19:40:40 2023, max compression
+gzip compressed data, was "ptcrossd-1.0.2.tar", last modified: Fri Aug  4 11:22:59 2023, max compression
```

## Comparing `ptcrossd-1.0.1.tar` & `ptcrossd-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-31 19:40:40.290927 ptcrossd-1.0.1/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    35823 2023-07-27 11:42:59.000000 ptcrossd-1.0.1/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3120 2023-07-31 19:40:40.286927 ptcrossd-1.0.1/PKG-INFO
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2633 2023-07-31 19:39:57.000000 ptcrossd-1.0.1/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-31 19:40:40.286927 ptcrossd-1.0.1/ptcrossd/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-27 11:42:59.000000 ptcrossd-1.0.1/ptcrossd/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-07-31 19:40:11.000000 ptcrossd-1.0.1/ptcrossd/_version.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8822 2023-07-31 19:40:16.000000 ptcrossd-1.0.1/ptcrossd/ptcrossd.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-31 19:40:40.286927 ptcrossd-1.0.1/ptcrossd.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3120 2023-07-31 19:40:40.000000 ptcrossd-1.0.1/ptcrossd.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      283 2023-07-31 19:40:40.000000 ptcrossd-1.0.1/ptcrossd.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-07-31 19:40:40.000000 ptcrossd-1.0.1/ptcrossd.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       52 2023-07-31 19:40:40.000000 ptcrossd-1.0.1/ptcrossd.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       33 2023-07-31 19:40:40.000000 ptcrossd-1.0.1/ptcrossd.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        9 2023-07-31 19:40:40.000000 ptcrossd-1.0.1/ptcrossd.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-07-31 19:40:40.290927 ptcrossd-1.0.1/setup.cfg
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1036 2023-07-27 11:42:59.000000 ptcrossd-1.0.1/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 11:22:59.458378 ptcrossd-1.0.2/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    35823 2023-07-27 11:42:59.000000 ptcrossd-1.0.2/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3151 2023-08-04 11:22:59.458378 ptcrossd-1.0.2/PKG-INFO
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2666 2023-08-03 16:40:19.000000 ptcrossd-1.0.2/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 11:22:59.458378 ptcrossd-1.0.2/ptcrossd/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-27 11:42:59.000000 ptcrossd-1.0.2/ptcrossd/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-08-03 16:41:44.000000 ptcrossd-1.0.2/ptcrossd/_version.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    12589 2023-08-03 17:50:01.000000 ptcrossd-1.0.2/ptcrossd/ptcrossd.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 11:22:59.458378 ptcrossd-1.0.2/ptcrossd.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3151 2023-08-04 11:22:59.000000 ptcrossd-1.0.2/ptcrossd.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      283 2023-08-04 11:22:59.000000 ptcrossd-1.0.2/ptcrossd.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-08-04 11:22:59.000000 ptcrossd-1.0.2/ptcrossd.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       52 2023-08-04 11:22:59.000000 ptcrossd-1.0.2/ptcrossd.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       33 2023-08-04 11:22:59.000000 ptcrossd-1.0.2/ptcrossd.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        9 2023-08-04 11:22:59.000000 ptcrossd-1.0.2/ptcrossd.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-08-04 11:22:59.458378 ptcrossd-1.0.2/setup.cfg
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1036 2023-07-27 11:42:59.000000 ptcrossd-1.0.2/setup.py
```

### Comparing `ptcrossd-1.0.1/LICENSE` & `ptcrossd-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ptcrossd-1.0.1/PKG-INFO` & `ptcrossd-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptcrossd
-Version: 1.0.1
+Version: 1.0.2
 Summary: crossdomain.xml misconfigurations testing tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -69,14 +69,16 @@
 defusedxml
 requests
 ptlibs
 ```
 
 ## Version History
 ```
+1.0.2
+    - Full script rework
 1.0.1
     - Fix urllib3 error
 1.0.0
     - updated for ptlibs 1.0.0
     - code refactorization
 0.0.1 - 0.0.2
     - Alpha releases
```

### Comparing `ptcrossd-1.0.1/README.md` & `ptcrossd-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 defusedxml
 requests
 ptlibs
 ```
 
 ## Version History
 ```
+1.0.2
+    - Full script rework
 1.0.1
     - Fix urllib3 error
 1.0.0
     - updated for ptlibs 1.0.0
     - code refactorization
 0.0.1 - 0.0.2
     - Alpha releases
```

### Comparing `ptcrossd-1.0.1/ptcrossd/ptcrossd.py` & `ptcrossd-1.0.2/ptcrossd/ptcrossd.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,114 +21,186 @@
 import argparse
 import re
 import sys; sys.path.append(__file__.rsplit("/", 1)[0])
 import urllib
 
 import requests
 import defusedxml.ElementTree as DEFUSED_ET
+import xml.etree.ElementTree as ET
 
 from _version import __version__
 from ptlibs import ptjsonlib, ptprinthelper, ptmisclib, ptnethelper
 
+
 class PtCrossd:
     def __init__(self, args):
-        self.ptjsonlib  = ptjsonlib.PtJsonLib()
-        self.headers    = ptnethelper.get_request_headers(args)
-        self.use_json   = args.json
-        self.timeout    = args.timeout
-        self.cache      = args.cache
-        self.proxies    = {"http": args.proxy, "https": args.proxy}
+        self.ptjsonlib   = ptjsonlib.PtJsonLib()
+        self.headers     = ptnethelper.get_request_headers(args)
+        self.use_json    = args.json
+        self.timeout     = args.timeout
+        self.cache       = args.cache
+        self.proxies     = {"http": args.proxy, "https": args.proxy}
+        self._validate_url(args.url)
+        self._set_tests(args)
+
+    def run(self, args) -> None:
+        if self.use_json:
+            if self.file_test:
+                url_path, url = self._adjust_url(args.url)
+                self._test_url(url, url_path)
+            if self.header_test:
+                self._test_headers_only(args.url)
+            self.ptjsonlib.set_status("ok")
+            ptprinthelper.ptprint(self.ptjsonlib.get_result_json())
+
+        else:
+            if self.file_test:
+                urls = self._get_paths_for_crossdomain(args.url)
+                for index, url in enumerate(urls):
+                    if index != 0: ptprinthelper.ptprint(" ", "", not self.use_json)
+                    self._test_url(url)
+            if not self.file_test and self.header_test:
+                self._test_headers_only(args.url)
 
-    def run(self, args):
-        rel_path, url = self._adjust_url(args.url)
+    def _test_headers_only(self, url) -> None:
         ptprinthelper.ptprint(f"Testing: {url}", "TITLE", not self.use_json, colortext=True)
+        response, response_dump = self._get_response(url)
+        if response.headers.get("Access-Control-Allow-Origin"):
+            if response.headers.get("Access-Control-Allow-Origin") == "*":
+                ptprinthelper.ptprint("Open CORS vulnerability detected in Access-Control-Allow-Origin header", "VULN", not self.use_json)
+                self.ptjsonlib.add_vulnerability("PTWV-OPEN-CORS-HEADER", request=response_dump["request"], response=response_dump["response"])
+        else:
+            ptprinthelper.ptprint(f'Header Access-Control-Allow-Origin is not present', "INFO", not self.use_json)
 
-        try:
-            response, response_dump = ptmisclib.load_url_from_web_or_temp(url, method="GET", headers=self.headers, proxies=self.proxies, timeout=self.timeout, redirects=False, verify=False, cache=self.cache, dump_response=True)
-        except requests.RequestException:
-            self.ptjsonlib.end_error(f"Cannot connect to server", self.use_json)
+    def _test_url(self, url, url_path=None) -> None:
+        ptprinthelper.ptprint(f"Testing: {url}", "TITLE", not self.use_json, colortext=True)
+        response, response_dump = self._get_response(url)
 
-        if response.status_code == 200:
+        ptprinthelper.ptprint(f"Returned Content-Type: '{response.headers.get('Content-Type')}'", "INFO", not self.use_json)
+        if self.header_test and not self.use_json:
             if response.headers.get("Access-Control-Allow-Origin"):
-                ptprinthelper.ptprint(f"Response Header: Access-Control-Allow-Origin: {response.headers.get('Access-Control-Allow-Origin')}", "INFO", not self.use_json)
-                if response.headers.get("Access-Control-Allow-Origin") == "*":
-                    self.ptjsonlib.add_vulnerability("PTWV-OPEN-CORS-HEADER", request=response_dump["request"], response=response_dump["response"])
-
-            if response.headers.get("Content-Type") in ["application/xml", "text/plain"]:
-                self.ptjsonlib.add_node(self.ptjsonlib.create_node_object("webpage", properties={"url": url, "name": rel_path[1:] if rel_path.startswith("/") else rel_path, "WebPageType": "crossdomain_xml"}))
-                self._process_crossdomain_xml(response, response_dump)
+                ptprinthelper.ptprint(f'Access-Control-Allow-Origin: {response.headers.get("Access-Control-Allow-Origin")}', "INFO", not self.use_json)
             else:
-                self.ptjsonlib.end_error(f"Expected Content-Type is application/xml, got {response.headers.get('Content-Type')}", self.use_json)
+                ptprinthelper.ptprint(f'Header Access-Control-Allow-Origin is not present', "INFO", not self.use_json)
+
+        if response.status_code == 200:
+            if self.use_json:
+                self.ptjsonlib.add_node(self.ptjsonlib.create_node_object("webpage", properties={"url": url, "name": url_path, "WebPageType": "crossdomain.xml"}))
+            self._process_crossdomain_xml(response, response_dump)
         else:
-            self.ptjsonlib.end_error(f"crossdomain.xml not found", self.use_json)
+            self.ptjsonlib.set_message("crossdomain.xml not found")
+            ptprinthelper.ptprint(f"crossdomain.xml not found", "INFO", not self.use_json)
 
-        if self.use_json:
-            ptprinthelper.ptprint(self.ptjsonlib.get_result_json())
+        if self.header_test and not self.use_json:
+            if response.headers.get("Access-Control-Allow-Origin"):
+                if response.headers.get("Access-Control-Allow-Origin") == "*":
+                    ptprinthelper.ptprint("Open CORS vulnerability detected in Access-Control-Allow-Origin header", "VULN", not self.use_json)
 
     def _process_crossdomain_xml(self, response, response_dump) -> None:
         try:
             tree = DEFUSED_ET.fromstring(response.text)
         except DEFUSED_ET.ParseError:
-            self.ptjsonlib.end_error("Error parsing provided XML file", self.use_json)
+            ptprinthelper.ptprint(f"Error parsing provided XML file", "ERROR", not self.use_json)
+            self.ptjsonlib.set_message("Error parsing provided XML file")
+            return
         except DEFUSED_ET.EntitiesForbidden:
-            self.ptjsonlib.end_error("Forbidden entities found, program will exit", self.use_json)
+            ptprinthelper.ptprint(f"Forbidden entities found", "ERROR", not self.use_json)
+            self.ptjsonlib.set_message("Forbidden entities found")
+            return
 
         if not self.use_json:
-            import xml.etree.ElementTree as ET
             element = ET.XML(response.text); ET.indent(element)
+            xml_string = ET.tostring(element, encoding='unicode')
             ptprinthelper.ptprint("XML content:", "TITLE", not self.use_json)
-            ptprinthelper.ptprint(ptprinthelper.get_colored_text(ET.tostring(element, encoding='unicode'), "INFO"), newline_above=True)
+            ptprinthelper.ptprint(ptprinthelper.get_colored_text(xml_string, "INFO"), condition=not self.use_json, newline_above=True)
 
-        self._allow_access_from_test(tree, response_dump)
+        ptprinthelper.ptprint(" ", "", not self.use_json)
+        self._run_allow_access_from_test(tree, response, response_dump)
 
-    def _allow_access_from_test(self, tree, response_dump) -> None:
-        has_open_cors = False
-        has_non_secure_communication = False
+    def _run_allow_access_from_test(self, tree, response, response_dump) -> None:
+        is_open_cors = False
+        http_allowed = False
         acf_elements = tree.findall("allow-access-from")
         if acf_elements:
             for acf_element in acf_elements:
                 if "domain" in acf_element.keys() and acf_element.attrib["domain"] == "*":
-                    has_open_cors = True
+                    is_open_cors = True
                 if "secure" in acf_element.keys() and not acf_element.attrib["secure"]:
-                    has_non_secure_communication = True
-            if has_open_cors:
-                ptprinthelper.ptprint("Open CORS vulnerability detected", "VULN", not self.use_json, newline_above=True)
-                self.ptjsonlib.add_vulnerability("PTWV-OPEN-CORS", request=response_dump["request"], response=response_dump["response"])
-            if has_non_secure_communication:
-                ptprinthelper.ptprint("Non-secure communication detected", "VULN", not self.use_json, newline_above=True)
-                self.ptjsonlib.add_vulnerability("PTWV-NON-SECURE-CORS", request=response_dump["request"], response=response_dump["response"])
-        else:
-            self.ptjsonlib.end_error("No allow-access-from elements were found", self.use_json)
+                    http_allowed = True
+            if is_open_cors:
+                ptprinthelper.ptprint("Open CORS vulnerability detected in crossdomain.xml file", "VULN", not self.use_json)
+                self.ptjsonlib.add_vulnerability("PTWV-OPEN-CORS-FILE", request=response_dump["request"], response=response_dump["response"])
+            if http_allowed:
+                ptprinthelper.ptprint("Non-secure communication detected in crossdomain.xml file", "VULN", not self.use_json)
 
+        if not is_open_cors:
+            self.ptjsonlib.set_message(response.text)
 
     def _adjust_url(self, url: str) -> tuple[str, str]:
         parsed_url = urllib.parse.urlparse(url)
-        if not re.match("https?$", parsed_url.scheme):
-            self.ptjsonlib.end_error("Missing or wrong scheme - only HTTP/HTTPS schemas are supported", self.use_json)
-        if not parsed_url.netloc:
-            self.ptjsonlib.end_error("Invalid URL provided", self.use_json)
-
         if not parsed_url.path.endswith("/crossdomain.xml"):
             if parsed_url.path in ["/", ""]:
                 parsed_url = parsed_url._replace(path="/crossdomain.xml")
             else:
-                parsed_url = parsed_url._replace(path='/'.join([i for i in parsed_url.path.split("/") if i]) + "/crossdomain.xml")
-        return (parsed_url.path, urllib.parse.urlunparse((parsed_url.scheme, parsed_url.netloc, parsed_url.path, "", "", "")))
+                directories = [d for d in parsed_url.path.split("/") if d]
+                if "." in directories[-1]:
+                    directories.pop()
+                parsed_url = parsed_url._replace(path='/'.join(directories) + "/crossdomain.xml")
+        return (parsed_url.path if not parsed_url.path.startswith("/") else parsed_url.path[1:], urllib.parse.urlunparse((parsed_url.scheme, parsed_url.netloc, parsed_url.path, "", "", "")))
+
+    def _get_paths_for_crossdomain(self, url) -> list:
+        parsed_url = urllib.parse.urlparse(url)
+        result = []
+        if parsed_url.path not in ["/", ""]:
+            directories = [d for d in parsed_url.path.split("/") if d]
+            if "." in directories[-1]:
+                directories.pop()
+            while directories:
+                path = '/'.join(directories) + "/crossdomain.xml"
+                result.append(urllib.parse.urlunparse((parsed_url.scheme, parsed_url.netloc, path, "", "", "")))
+                directories.pop()
+        result.append(urllib.parse.urlunparse((parsed_url.scheme, parsed_url.netloc, "/crossdomain.xml", "", "", "")))
+        return result
+
+    def _validate_url(self, url: str) -> None:
+        parsed_url = urllib.parse.urlparse(url)
+        if not re.match("https?$", parsed_url.scheme):
+            self.ptjsonlib.end_error("Missing or wrong scheme, only HTTP(s) schemas are supported", self.use_json)
+        if not parsed_url.netloc:
+            self.ptjsonlib.end_error("Provided URL is not valid", self.use_json)
+
+    def _set_tests(self, args) -> None:
+        if not args.cross_domain_file and not args.cross_origin_header:
+            self.header_test = True
+            self.file_test = True
+        else:
+            self.file_test = args.cross_domain_file
+            self.header_test = args.cross_origin_header
+
+    def _get_response(self, url: str):
+        try:
+            response, response_dump = ptmisclib.load_url_from_web_or_temp(url, method="GET", headers=self.headers, proxies=self.proxies, timeout=self.timeout, redirects=False, verify=False, cache=self.cache, dump_response=True)
+            return response, response_dump
+        except requests.RequestException:
+            self.ptjsonlib.end_error(f"Cannot connect to server", self.use_json)
 
 
 def get_help():
     return [
         {"description": ["crossdomain.xml misconfigurations testing tool"]},
         {"usage": ["ptcrossd <options>"]},
         {"usage_example": [
             "ptcrossd -u https://www.example.com/crossdomain.xml",
-            "ptcrossd -u https://www.example.com/"
+            "ptcrossd -u https://www.example.com/",
+
         ]},
         {"options": [
             ["-u",  "--url",                    "<url>",            "Connect to URL"],
+            ["-cf",  "--cross-domain-file",     "",                 "Test crossdomain.xml file"],
+            ["-ch", "--cross-origin-header",    "",                 "Test Access-Control-Allow-Origin header"],
             ["-p",  "--proxy",                  "<proxy>",          "Set proxy (e.g. http://127.0.0.1:8080)"],
             ["-T",  "--timeout",                "<timeout>",        "Set timeout (default to 10)"],
             ["-c",  "--cookie",                 "<cookie>",         "Set cookie"],
             ["-ua", "--user-agent",             "<user-agent>",     "Set User-Agent header"],
             ["-H",  "--headers",                "<header:value>",   "Set custom header(s)"],
             ["-C",  "--cache",                  "",                 "Cache requests (load from tmp in future)"],
             ["-v",  "--version",                "",                 "Show script version and exit"],
@@ -136,23 +208,25 @@
             ["-j",  "--json",                   "",                 "Output in JSON format"],
         ]
         }]
 
 
 def parse_args():
     parser = argparse.ArgumentParser(add_help="False")
-    parser.add_argument("-u",  "--url",         type=str, required=True)
-    parser.add_argument("-p",  "--proxy",       type=str)
-    parser.add_argument("-c",  "--cookie",      type=str)
-    parser.add_argument("-ua", "--user-agent",  type=str, default="Penterep Tools")
-    parser.add_argument("-T",  "--timeout",     type=int, default=10)
-    parser.add_argument("-H",  "--headers",     type=ptmisclib.pairs, nargs="+")
-    parser.add_argument("-j",  "--json",        action="store_true")
-    parser.add_argument("-C",  "--cache",       action="store_true")
-    parser.add_argument("-v",  "--version",     action="version", version=f"{SCRIPTNAME} {__version__}")
+    parser.add_argument("-u",   "--url",                 type=str, required=True)
+    parser.add_argument("-p",   "--proxy",               type=str)
+    parser.add_argument("-c",   "--cookie",              type=str)
+    parser.add_argument("-ua",  "--user-agent",          type=str, default="Penterep Tools")
+    parser.add_argument("-T",   "--timeout",             type=int, default=10)
+    parser.add_argument("-H",   "--headers",             type=ptmisclib.pairs, nargs="+")
+    parser.add_argument("-cf",  "--cross-domain-file",   action="store_true")
+    parser.add_argument("-ch",  "--cross-origin-header", action="store_true")
+    parser.add_argument("-j",   "--json",                action="store_true")
+    parser.add_argument("-C",   "--cache",               action="store_true")
+    parser.add_argument("-v",   "--version",             action="version", version=f"{SCRIPTNAME} {__version__}")
 
     if len(sys.argv) == 1 or "-h" in sys.argv or "--help" in sys.argv:
         ptprinthelper.help_print(get_help(), SCRIPTNAME, __version__)
         sys.exit(0)
 
     args = parser.parse_args()
     ptprinthelper.print_banner(SCRIPTNAME, __version__, args.json)
```

### Comparing `ptcrossd-1.0.1/ptcrossd.egg-info/PKG-INFO` & `ptcrossd-1.0.2/ptcrossd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptcrossd
-Version: 1.0.1
+Version: 1.0.2
 Summary: crossdomain.xml misconfigurations testing tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -69,14 +69,16 @@
 defusedxml
 requests
 ptlibs
 ```
 
 ## Version History
 ```
+1.0.2
+    - Full script rework
 1.0.1
     - Fix urllib3 error
 1.0.0
     - updated for ptlibs 1.0.0
     - code refactorization
 0.0.1 - 0.0.2
     - Alpha releases
```

### Comparing `ptcrossd-1.0.1/setup.py` & `ptcrossd-1.0.2/setup.py`

 * *Files identical despite different names*

