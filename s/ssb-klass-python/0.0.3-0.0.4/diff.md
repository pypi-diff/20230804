# Comparing `tmp/ssb_klass_python-0.0.3.tar.gz` & `tmp/ssb_klass_python-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_klass_python-0.0.3.tar", max compression
+gzip compressed data, was "ssb_klass_python-0.0.4.tar", max compression
```

## Comparing `ssb_klass_python-0.0.3.tar` & `ssb_klass_python-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1076 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/LICENSE.md
--rw-r--r--   0        0        0     1556 2023-05-16 11:03:15.361497 ssb_klass_python-0.0.3/README.md
--rw-r--r--   0        0        0     1487 2023-05-16 11:03:15.361497 ssb_klass_python-0.0.3/klass/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/classes/__init__.py
--rw-r--r--   0        0        0     3229 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/classes/classification.py
--rw-r--r--   0        0        0     3857 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/classes/codes.py
--rw-r--r--   0        0        0     2233 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/classes/correspondance.py
--rw-r--r--   0        0        0      704 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/classes/family.py
--rw-r--r--   0        0        0     3810 2023-05-16 11:03:15.361497 ssb_klass_python-0.0.3/klass/classes/search.py
--rw-r--r--   0        0        0     2293 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/classes/variant.py
--rw-r--r--   0        0        0     1831 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/classes/version.py
--rw-r--r--   0        0        0      551 2023-05-16 11:03:15.361497 ssb_klass_python-0.0.3/klass/klass_config.py
--rw-r--r--   0        0        0        0 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/requests/__init__.py
--rw-r--r--   0        0        0    11092 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/requests/klass_requests.py
--rw-r--r--   0        0        0      530 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/requests/sections.py
--rw-r--r--   0        0        0     3121 2023-05-16 11:03:15.361497 ssb_klass_python-0.0.3/klass/requests/validate.py
--rw-r--r--   0        0        0        0 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/samples/__init__.py
--rw-r--r--   0        0        0      180 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/utility/classification.py
--rw-r--r--   0        0        0      244 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/utility/codes.py
--rw-r--r--   0        0        0        0 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/widgets/__init__.py
--rw-r--r--   0        0        0     3078 2023-05-16 11:03:15.361497 ssb_klass_python-0.0.3/klass/widgets/search_ipywidget.py
--rw-r--r--   0        0        0     1156 2023-05-16 11:03:15.361497 ssb_klass_python-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2220 1970-01-01 00:00:00.000000 ssb_klass_python-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0     1722 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/README.md
+-rw-r--r--   0        0        0     1488 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/klass/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/classes/__init__.py
+-rw-r--r--   0        0        0     3913 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/klass/classes/classification.py
+-rw-r--r--   0        0        0     4459 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/klass/classes/codes.py
+-rw-r--r--   0        0        0     3423 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/klass/classes/correspondance.py
+-rw-r--r--   0        0        0      704 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/classes/family.py
+-rw-r--r--   0        0        0     3810 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/classes/search.py
+-rw-r--r--   0        0        0     2631 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/klass/classes/variant.py
+-rw-r--r--   0        0        0     1831 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/classes/version.py
+-rw-r--r--   0        0        0      520 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/klass/klass_config.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/requests/__init__.py
+-rw-r--r--   0        0        0    10886 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/klass/requests/klass_requests.py
+-rw-r--r--   0        0        0      530 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/requests/sections.py
+-rw-r--r--   0        0        0     3199 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/klass/requests/validate.py
+-rw-r--r--   0        0        0      180 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/utility/classification.py
+-rw-r--r--   0        0        0      244 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/utility/codes.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/widgets/__init__.py
+-rw-r--r--   0        0        0     3078 2023-08-04 09:38:06.148982 ssb_klass_python-0.0.4/klass/widgets/search_ipywidget.py
+-rw-r--r--   0        0        0     1156 2023-08-04 09:38:25.605431 ssb_klass_python-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2386 1970-01-01 00:00:00.000000 ssb_klass_python-0.0.4/PKG-INFO
```

### Comparing `ssb_klass_python-0.0.3/LICENSE.md` & `ssb_klass_python-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.3/README.md` & `ssb_klass_python-0.0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -4,29 +4,35 @@
 The package aims to make Klass's API for retrieving data easier to use by re-representing Klass's internal hierarchy as python-classes. Containing methods for easier traversal down, search classes and widgets, reasonable defaults to parameters etc.
 Where data is possible to fit into pandas DataFrames, this will be preferred, but hirerachical data will be kept as json / dict structure.
 
 
 ## Example usages
 
 
+### Getting started
 ```python
 from klass import search_classification
 # Opens a ipywidget in notebooks for searching for classifications and copying code, to get started
 search_classification(no_dupes=True)
 ```
 
+### Getting a classification directly
 ```python
 from klass import get_classification # Import the utility-function
 nus = get_classification(36)
 ```
 
 ```python
 # Does the same as the code above, but does not shy away from using the class directly
 from klass import KlassClassification # Import the class for KlassClassifications
 nus = KlassClassification(36)  # Use ID for classification
+```
+
+When you have the classification stored in an object, you can "dig into" the API from there.
+```python
 codes = nus.get_codes() # codes from current date
 print(codes)
 codes.data  # Pandas dataframe available under the .data attribute
 ```
```

### Comparing `ssb_klass_python-0.0.3/klass/__init__.py` & `ssb_klass_python-0.0.4/klass/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib import import_module
 
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __all__ = []
 
 # Everything we want to be directly importable from under "klass"-package
 local_imports = {
     "requests.klass_requests": [
         "classifications",
         "classification_search",
@@ -25,15 +25,15 @@
     ],
     "classes.codes": ["KlassCodes"],
     "classes.correspondance": ["KlassCorrespondance"],
     "classes.classification": ["KlassClassification"],
     "classes.family": ["KlassFamily"],
     "classes.search": ["KlassSearchClassifications", "KlassSearchFamilies"],
     "requests.sections": ["sections_list", "sections_dict"],
-    "classes.variant": ["KlassVariant", "KlassVariantCodes"],
+    "classes.variant": ["KlassVariant", "KlassVariantSearch"],
     "classes.version": ["KlassVersion"],
     "utility.codes": ["get_codes"],
     "utility.classification": ["get_classification"],
     "widgets.search_ipywidget": ["search_classification"],
     "klass_config": ["KlassConfig"],
 }
```

### Comparing `ssb_klass_python-0.0.3/klass/classes/classification.py` & `ssb_klass_python-0.0.4/klass/classes/classification.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from ..requests.klass_requests import classification_by_id
+import pandas as pd
+
+from ..requests.klass_requests import changes, classification_by_id
 from .codes import KlassCodes
 from .correspondance import KlassCorrespondance
 from .variant import KlassVariant
 from .version import KlassVersion
 
 
 class KlassClassification:
@@ -80,23 +82,44 @@
             include_future=include_future,
         )
 
     def get_codes(
         self,
         from_date: str = "",
         to_date: str = "",
+        select_codes: str = "",
+        select_level: str = "",
+        presentation_name_pattern: str = "",
         language: str = "",
         include_future: bool = None,
     ) -> KlassCodes:
         # If not passed to method, grab these from the Classification
         if language == "":
             language = self.language
         if include_future is None:
             include_future = self.include_future
 
         return KlassCodes(
             classification_id=self.classification_id,
             from_date=from_date,
             to_date=to_date,
+            select_codes=select_codes,
+            select_level=select_level,
+            presentation_name_pattern=presentation_name_pattern,
+            language=language,
+            include_future=include_future,
+        )
+
+    def get_changes(
+        self,
+        from_date: str,
+        to_date: str = "",
+        language: str = "nb",
+        include_future: bool = False,
+    ) -> pd.DataFrame:
+        return changes(
+            classification_id=self.classification_id,
+            from_date=from_date,
+            to_date=to_date,
             language=language,
             include_future=include_future,
         )
```

### Comparing `ssb_klass_python-0.0.3/klass/classes/codes.py` & `ssb_klass_python-0.0.4/klass/classes/codes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import defaultdict
 from datetime import datetime
 
 from ..requests.klass_requests import codes, codes_at
 
 
 class KlassCodes:
     def __init__(
@@ -102,9 +103,26 @@
                 select_codes=self.select_codes,
                 select_level=self.select_level,
                 presentation_name_pattern=self.presentation_name_pattern,
                 language=self.language,
                 include_future=self.include_future,
             )
 
+    def to_dict(
+        self,
+        key: str = "code",
+        value: str = "",  # default is "name" if not set
+        other: str = "",
+    ) -> dict | defaultdict:
+        if not value:
+            # If you bothered specifying a pattern, we assume you want it
+            if self.presentation_name_pattern:
+                value = "presentationName"
+            else:
+                value = "name"
+        mapping = dict(zip(self.data[key], self.data[value]))
+        if other:
+            mapping = defaultdict(lambda: other, mapping)
+        return mapping
+
     def wide_data(self):
         return self.data.pivot_table("level")
```

### Comparing `ssb_klass_python-0.0.3/klass/classes/correspondance.py` & `ssb_klass_python-0.0.4/klass/classes/variant.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,79 @@
-from ..requests.klass_requests import correspondance_table_by_id, corresponds
 import pandas as pd
 
+from ..requests.klass_requests import variant, variant_at, variants_by_id
 
-class KlassCorrespondance:
+
+class KlassVariant:
+    def __init__(
+        self,
+        variant_id: str,
+        language: str = "nb",
+    ):
+        self.variant_id = variant_id
+        self.language = language
+        for key, value in variants_by_id(self.variant_id, self.language).items():
+            setattr(self, key, value)
+
+    def get_classification_codes(self, select_level: int = 0) -> pd.DataFrame:
+        df = pd.json_normalize(self.classificationItems)
+        if select_level:
+            return df[df["level"] == str(select_level)]
+        return df
+
+
+class KlassVariantSearch:
     def __init__(
         self,
-        correspondance_id: str = "",
-        source_classification_id: str = "",
-        target_classification_id: str = "",
-        from_date: str = "",
+        classification_id: str,
+        variant_name: str,
+        from_date: str,
         to_date: str = "",
+        select_codes: str = "",
+        select_level: str = "",
+        presentation_name_pattern: str = "",
         language: str = "nb",
         include_future: bool = False,
     ):
-        self.correspondance_id = correspondance_id
-        self.source_classification_id = source_classification_id
-        self.target_classification_id = target_classification_id
+        self.classification_id = classification_id
+        self.variant_name = variant_name
         self.from_date = from_date
         self.to_date = to_date
+        self.select_codes = (select_codes,)
+        self.select_level = (select_level,)
+        self.presentation_name_pattern = presentation_name_pattern
         self.language = language
         self.include_future = include_future
 
-        if correspondance_id:
-            self.data = correspondance_table_by_id(
-                correspondance_id, language=language
-            )
-        elif source_classification_id and target_classification_id and from_date:
-            self.data = corresponds(
-                source_classification_id=source_classification_id,
-                target_classification_id=target_classification_id,
-                from_date=from_date,
-                to_date=to_date,
-                language=language,
-                include_future=include_future,
+        if self.to_date:
+            self.data = variant(
+                classification_id=self.classification_id,
+                variant_name=self.variant_name,
+                from_date=self.from_date,
+                to_date=self.to_date,
+                select_codes=self.select_codes,
+                select_level=self.select_level,
+                presentation_name_pattern=self.presentation_name_pattern,
+                language=self.language,
+                include_future=self.include_future,
             )
         else:
-            raise ValueError(
-                "Please set correspondance ID, or source and target classification IDs + from_date"
+            self.data = variant_at(
+                classification_id=self.classification_id,
+                variant_name=self.variant_name,
+                date=self.from_date,
+                select_codes=self.select_codes,
+                select_level=self.select_level,
+                presentation_name_pattern=self.presentation_name_pattern,
+                language=self.language,
+                include_future=self.include_future,
             )
 
-    def __str__(self):
-        return str(self.__dict__)
-
-    def __repr__(self):
-        result = "KlassCorrespondance("
-        if self.correspondance_id:
-            result += f"correspondance_id={self.correspondance_id}, "
-        if self.source_classification_id:
-            result += f"source_classification_id={self.source_classification_id}, "
-        if self.target_classification_id:
-            result += f"target_classification_id={self.target_classification_id}, "
-        if self.from_date:
-            result += f"from_date={self.from_date}, "
-        if self.to_date:
-            result += f"to_date={self.to_date}, "
-        if self.language != "nb":
-            result += f"language={self.language}, "
-        result += ")"
-        return result
+        @staticmethod
+        def get_variant(
+            variant_id: str,
+            language: str = "nb",
+        ) -> KlassVariant:
+            return KlassVariant(
+                variant_id=variant_id,
+                language=language,
+            )
```

### Comparing `ssb_klass_python-0.0.3/klass/classes/family.py` & `ssb_klass_python-0.0.4/klass/classes/family.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.3/klass/classes/search.py` & `ssb_klass_python-0.0.4/klass/classes/search.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.3/klass/classes/version.py` & `ssb_klass_python-0.0.4/klass/classes/version.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.3/klass/klass_config.py` & `ssb_klass_python-0.0.4/klass/klass_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-class Singleton():
+class Singleton:
     def __new__(cls, *args, **kwds):
         it = cls.__dict__.get("__it__")
         if it is not None:
             return it
         cls.__it__ = it = object.__new__(cls)
         it.singleton_init(*args, **kwds)
         return it
 
 
 class KlassConfig(Singleton):
     def singleton_init(self):
         self.LANGUAGES = ["nb", "nn", "en"]
         self.BASE_URL = "https://data.ssb.no/api/klass/v1/"
         self.HEADERS = {
-            "Accept": 'application/json',
+            "Accept": "application/json",
         }
         self.TESTING = False
-        self.MOCKING = False
```

### Comparing `ssb_klass_python-0.0.3/klass/requests/klass_requests.py` & `ssb_klass_python-0.0.4/klass/requests/klass_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,22 +19,32 @@
     if KlassConfig().TESTING:
         print("Full URL, check during testing:", req.prepare().url)
     response = requests.Session().send(req.prepare())
     response.raise_for_status()
     return response.json()
 
 
+def get_text(url, params):
+    req = requests.Request("GET", url=url, headers=KlassConfig().HEADERS, params=params)
+    if KlassConfig().TESTING:
+        print("Full URL, check during testing:", req.prepare().url)
+    response = requests.Session().send(req.prepare())
+    response.raise_for_status()
+    return response.text
+
+
 def convert_return_type(data, return_type="pandas"):
     if return_type == "json":
         return data
     return pd.json_normalize(data)
 
 
 def convert_datestring(date: str, return_type="isoklass") -> str:
-    date = dateutil.parser.parse(date)
+    if isinstance(date, str):
+        date = dateutil.parser.parse(date)
     date = date.replace(tzinfo=timezone(timedelta(hours=1)))
     if return_type == "isoklass":
         return date.strftime("%Y-%m-%dT%H:%M:%S.%f")[:-3] + date.strftime("%z")
     elif return_type == "yyyy-mm-dd":
         return date.strftime("%Y-%m-%d")
     raise ValueError("Unrecognized datetimestring return type")
 
@@ -46,60 +56,66 @@
 
 
 # ############
 # ENDPOINTS #
 # ############
 
 
-def classifications(include_codelists: bool = False,
-                    changed_since: str = ""):
+def classifications(include_codelists: bool = False, changed_since: str = ""):
     url = KlassConfig().BASE_URL + "classifications"
-    params = {'includeCodelists': include_codelists, }
+    params = {
+        "includeCodelists": include_codelists,
+    }
     if changed_since:
         params["changedSince"] = convert_datestring(changed_since, "isoklass")
     params = validate_params(params)
     return get_json(url, params)
 
 
-def classification_search(query: str = "",
-                          include_codelists: bool = False,
-                          ssbsection: str = ""):
+def classification_search(
+    query: str = "", include_codelists: bool = False, ssbsection: str = ""
+):
     url = KlassConfig().BASE_URL + "classifications/search"
     if not query:
         raise ValueError("Please specify a query")
     params = {
         "query": query,
         "includeCodelists": include_codelists,
     }
     if ssbsection:
         params["ssbSection"] = convert_section(ssbsection)
     params = validate_params(params)
     return get_json(url, params)
 
 
-def classification_by_id(classification_id: str,
-                         language: str = 'nb', 
-                         include_future: bool = False,
-                         return_type: str = "json") -> dict:
+def classification_by_id(
+    classification_id: str,
+    language: str = "nb",
+    include_future: bool = False,
+    return_type: str = "json",
+) -> dict:
     url = KlassConfig().BASE_URL + "classifications/" + str(classification_id)
-    params = validate_params({'language': language,
-                              'includeFuture': include_future})
+    params = validate_params({"language": language, "includeFuture": include_future})
     return convert_return_type(get_json(url, params), return_type)
 
 
-def codes(classification_id: str,
-          from_date: str,
-          to_date: str = "",
-          select_codes: str = "",
-          select_level: str = "",
-          presentation_name_pattern: str = "",
-          language: str = "nb",
-          include_future: bool = False,
-          return_type: str = "pandas") -> pd.DataFrame:
-    url = KlassConfig().BASE_URL + "classifications/" + str(classification_id) + "/codes"
+def codes(
+    classification_id: str,
+    from_date: str,
+    to_date: str = "",
+    select_codes: str = "",
+    select_level: str = "",
+    presentation_name_pattern: str = "",
+    language: str = "nb",
+    include_future: bool = False,
+    return_type: str = "pandas",
+) -> pd.DataFrame:
+    url = (
+        KlassConfig().BASE_URL + "classifications/" + str(classification_id) + "/codes"
+    )
     from_date = convert_datestring(from_date, "yyyy-mm-dd")
     params = {
         "from": from_date,
         "selectCodes": select_codes,
         "selectLevel": select_level,
         "presentationNamePattern": presentation_name_pattern,
         "language": language,
@@ -108,58 +124,77 @@
     if to_date:
         params["to"] = convert_datestring(to_date)
         params["to"] = to_date
     params = validate_params({k: v for k, v in params.items() if v != ""})
     return convert_return_type(get_json(url, params)["codes"], return_type)
 
 
-def codes_at(classification_id: str,
-             date: str,
-             select_codes: str = "",
-             select_level: str = "",
-             presentation_name_pattern: str = "",
-             language: str = "nb",
-             include_future: bool = False,
-             return_type: str = "pandas"):
-    url = KlassConfig().BASE_URL + "classifications/" + str(classification_id) + "/codesAt"
+def codes_at(
+    classification_id: str,
+    date: str,
+    select_codes: str = "",
+    select_level: str = "",
+    presentation_name_pattern: str = "",
+    language: str = "nb",
+    include_future: bool = False,
+    return_type: str = "pandas",
+):
+    url = (
+        KlassConfig().BASE_URL
+        + "classifications/"
+        + str(classification_id)
+        + "/codesAt"
+    )
     date = convert_datestring(date, "yyyy-mm-dd")
     params = {
         "date": date,
         "selectCodes": select_codes,
         "selectLevel": select_level,
         "presentationNamePattern": presentation_name_pattern,
         "language": language,
         "includeFuture": include_future,
     }
     params = validate_params({k: v for k, v in params.items() if v != ""})
     return convert_return_type(get_json(url, params)["codes"], return_type)
 
-def version_by_id(version_id: str,
-                  language: str = "nb",
-                  include_future: bool = False,
-                  return_type: str = "json"):
+
+def version_by_id(
+    version_id: str,
+    language: str = "nb",
+    include_future: bool = False,
+    return_type: str = "json",
+):
     url = KlassConfig().BASE_URL + "versions/" + str(version_id)
-    params = validate_params({
-        'language': language,
-        'includeFuture': include_future,
-    })
+    params = validate_params(
+        {
+            "language": language,
+            "includeFuture": include_future,
+        }
+    )
     return convert_return_type(get_json(url, params), return_type)
 
 
-def variant(classification_id: str,
-            variant_name: str,
-            from_date: str,
-            to_date: str = "",
-            select_codes: str = "",
-            select_level: str = "",
-            presentation_name_pattern: str = "",
-            language: str = "nb",
-            include_future: bool = False,
-            return_type: str = "pandas"):
-    url = KlassConfig().BASE_URL + "classifications/" + str(classification_id) + "/variant"
+def variant(
+    classification_id: str,
+    variant_name: str,
+    from_date: str,
+    to_date: str = "",
+    select_codes: str = "",
+    select_level: str = "",
+    presentation_name_pattern: str = "",
+    language: str = "nb",
+    include_future: bool = False,
+    return_type: str = "pandas",
+):
+    url = (
+        KlassConfig().BASE_URL
+        + "classifications/"
+        + str(classification_id)
+        + "/variant"
+    )
     from_date = convert_datestring(from_date, "yyyy-mm-dd")
     params = {
         "variantName": variant_name,
         "from": from_date,
         "selectCodes": select_codes,
         "selectLevel": select_level,
         "presentationNamePattern": presentation_name_pattern,
@@ -169,132 +204,162 @@
     if to_date:
         params["to"] = convert_datestring(to_date, "yyyy-mm-dd")
     params = validate_params({k: v for k, v in params.items() if v != ""})
     print(params)
     return convert_return_type(get_json(url, params)["codes"], return_type)
 
 
-def variant_at(classification_id: str,
-               variant_name: str,
-               date: str,
-               select_codes: str = "",
-               select_level: str = "",
-               presentation_name_pattern: str = "",
-               language: str = "nb",
-               include_future: bool = False,
-               return_type: str = "pandas"):
-    url = KlassConfig().BASE_URL + "classifications/" + str(classification_id) + "/variantAt"
+def variant_at(
+    classification_id: str,
+    variant_name: str,
+    date: str,
+    select_codes: str = "",
+    select_level: str = "",
+    presentation_name_pattern: str = "",
+    language: str = "nb",
+    include_future: bool = False,
+    return_type: str = "pandas",
+):
+    url = (
+        KlassConfig().BASE_URL
+        + "classifications/"
+        + str(classification_id)
+        + "/variantAt"
+    )
     date = convert_datestring(date, "yyyy-mm-dd")
     params = {
         "variantName": variant_name,
         "date": date,
         "selectCodes": select_codes,
         "selectLevel": select_level,
         "presentationNamePattern": presentation_name_pattern,
         "language": language,
         "includeFuture": include_future,
     }
-    params = validate_params({k: v for k, v in params.items() if v != ""})
+    params = validate_params({k: v for k, v in params.items() if v not in ["", ("",)]})
     return convert_return_type(get_json(url, params)["codes"], return_type)
 
 
-def variants_by_id(variant_id: str,
-                  language: str = "nb",
-                  return_type: str = "json"
-                  ):
+def variants_by_id(variant_id: str, language: str = "nb", return_type: str = "json"):
     url = KlassConfig().BASE_URL + "variants/" + str(variant_id)
-    params = validate_params({'language': language})
+    params = validate_params({"language": language})
     return convert_return_type(get_json(url, params), return_type)
 
 
-def corresponds(source_classification_id: str,
-                target_classification_id: str,
-                from_date: str,
-                to_date: str = "",
-                language: str = "nb",
-                include_future: bool = False,
-                return_type: str = "pandas"):
-    url = KlassConfig().BASE_URL + "classifications/" + str(source_classification_id) + "/corresponds"
+def corresponds(
+    source_classification_id: str,
+    target_classification_id: str,
+    from_date: str,
+    to_date: str = "",
+    language: str = "nb",
+    include_future: bool = False,
+    return_type: str = "json",
+):
+    url = (
+        KlassConfig().BASE_URL
+        + "classifications/"
+        + str(source_classification_id)
+        + "/corresponds"
+    )
     from_date = convert_datestring(from_date, "yyyy-mm-dd")
     params = {
         "targetClassificationId": target_classification_id,
         "from": from_date,
         "language": language,
         "includeFuture": include_future,
     }
     if to_date:
         params["to"] = convert_datestring(to_date, "yyyy-mm-dd")
     params = validate_params({k: v for k, v in params.items() if v != ""})
 
-    return convert_return_type(get_json(url, params)['correspondenceItems'], return_type)
+    return convert_return_type(get_json(url, params), return_type)
 
 
-def corresponds_at(source_classification_id: str,
-                   target_classification_id: str,
-                   date: str,
-                   language: str = "nb",
-                   include_future: bool = False,
-                   return_type: str = "pandas"):
-    url = KlassConfig().BASE_URL + "classifications/" + str(source_classification_id) + "/correspondsAt"
+def corresponds_at(
+    source_classification_id: str,
+    target_classification_id: str,
+    date: str,
+    language: str = "nb",
+    include_future: bool = False,
+    return_type: str = "json",
+):
+    url = (
+        KlassConfig().BASE_URL
+        + "classifications/"
+        + str(source_classification_id)
+        + "/correspondsAt"
+    )
     date = convert_datestring(date, "yyyy-mm-dd")
     params = {
         "targetClassificationId": target_classification_id,
         "date": date,
         "language": language,
         "includeFuture": include_future,
     }
     params = validate_params({k: v for k, v in params.items() if v != ""})
-    return convert_return_type(
-        get_json(url, params)["correspondenceItems"], return_type
-    )
+    return convert_return_type(get_json(url, params), return_type)
 
 
-def correspondance_table_by_id(correspondance_id: str,
-                               language: str = "nb",
-                               return_type: str = "json"):
+def correspondance_table_by_id(
+    correspondance_id: str, language: str = "nb", return_type: str = "json"
+):
     url = KlassConfig().BASE_URL + "correspondencetables/" + str(correspondance_id)
-    params = validate_params({'language': language})
+    params = validate_params({"language": language})
     return convert_return_type(get_json(url, params), return_type)
 
 
-def changes(classification_id: str,
-            from_date: str,
-            to_date: str = "",
-            language: str = "nb",
-            include_future: bool = False,
-            return_type: str = "pandas"
-           ):
-    url = KlassConfig().BASE_URL + "classifications/" + str(classification_id) + "/changes"
+def changes(
+    classification_id: str,
+    from_date: str,
+    to_date: str = "",
+    language: str = "nb",
+    include_future: bool = False,
+    return_type: str = "pandas",
+):
+    url = (
+        KlassConfig().BASE_URL
+        + "classifications/"
+        + str(classification_id)
+        + "/changes.json"
+    )
     from_date = convert_datestring(from_date, "yyyy-mm-dd")
-    to_date = convert_datestring(to_date, "yyyy-mm-dd")
+    if to_date:
+        to_date = convert_datestring(to_date, "yyyy-mm-dd")
     params = {
         "from": from_date,
         "to": to_date,
         "language": language,
         "includeFuture": include_future,
     }
     params = validate_params({k: v for k, v in params.items() if v != ""})
     return convert_return_type(get_json(url, params)["codeChanges"], return_type)
 
 
-def classificationfamilies(ssbsection: str = "",
-                           include_codelists: bool = False,
-                           language: str = "nb",
-                           ):
+def classificationfamilies(
+    ssbsection: str = "",
+    include_codelists: bool = False,
+    language: str = "nb",
+):
     url = KlassConfig().BASE_URL + "classificationfamilies"
-    params = {'includeCodelists': include_codelists, 'language': language}
+    params = {"includeCodelists": include_codelists, "language": language}
     if ssbsection:
         params["ssbSection"] = convert_section(ssbsection)
     params = validate_params(params)
     return get_json(url, params)
 
 
-def classificationfamilies_by_id(classificationfamily_id: str,
-                                 ssbsection: str = "",
-                                 include_codelists: bool = False,
-                                 language: str = "nb",):
-    url = KlassConfig().BASE_URL + "classificationfamilies/" + str(classificationfamily_id)
-    params = {'includeCodelists': include_codelists, 'language': language}
+def classificationfamilies_by_id(
+    classificationfamily_id: str,
+    ssbsection: str = "",
+    include_codelists: bool = False,
+    language: str = "nb",
+):
+    url = (
+        KlassConfig().BASE_URL
+        + "classificationfamilies/"
+        + str(classificationfamily_id)
+    )
+    params = {"includeCodelists": include_codelists, "language": language}
     if ssbsection:
         params["ssbSection"] = convert_section(ssbsection)
     params = validate_params(params)
     return get_json(url, params)
```

### Comparing `ssb_klass_python-0.0.3/klass/requests/sections.py` & `ssb_klass_python-0.0.4/klass/requests/sections.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.3/klass/requests/validate.py` & `ssb_klass_python-0.0.4/klass/requests/validate.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,17 @@
         raise ValueError("Incorrect data format, should be YYYY-MM-DD")
     return date
 
 
 def validate_language(language: str) -> str:
     language = language.lower()
     if language not in KlassConfig().LANGUAGES:
-        raise ValueError(f"Specify one of the valid languages: {', '.join(LANGUAGES)}")
+        raise ValueError(
+            f"Specify one of the valid languages: {', '.join(KlassConfig().LANGUAGES)}"
+        )
     return language
 
 
 def validate_bool(val: bool) -> bool:
     if type(val) != bool:
         raise TypeError(f"{val} needs to be a bool")
     val = str(val).lower()
@@ -72,17 +74,18 @@
     check = "".join([c for c in pattern if c not in remove])
     if not check.isalpha():
         raise ValueError("Unexpected characters in presentation name pattern.")
     return pattern
 
 
 def validate_alnum_spaces(variant_name: str) -> str:
-    check = variant_name.replace(" ", "")
-    #print(f"{check=}")
-    if not check in ["", " "] and not check.isalnum() :
+    check = (
+        variant_name.replace(" ", "").replace("(", "").replace(")", "").replace("-", "")
+    )
+    if check not in ["", " "] and not check.isalnum():
         raise ValueError(
             "Expecting variant name to only include numbers, characters and spaces..."
         )
     return variant_name
 
 
 def validate_time_iso8601(datestring: str) -> str:
```

### Comparing `ssb_klass_python-0.0.3/klass/widgets/search_ipywidget.py` & `ssb_klass_python-0.0.4/klass/widgets/search_ipywidget.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.3/pyproject.toml` & `ssb_klass_python-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-klass-python"
-version = "0.0.3"
+version = "0.0.4"
 description = "A Python package built on top of KLASS's API for retrieving classifications, codes, correspondances etc."
 authors = ["Carl Corneil <cfc@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "klass"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ssb_klass_python-0.0.3/PKG-INFO` & `ssb_klass_python-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-klass-python
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package built on top of KLASS's API for retrieving classifications, codes, correspondances etc.
 License: MIT
 Author: Carl Corneil
 Author-email: cfc@ssb.no
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,29 +22,35 @@
 The package aims to make Klass's API for retrieving data easier to use by re-representing Klass's internal hierarchy as python-classes. Containing methods for easier traversal down, search classes and widgets, reasonable defaults to parameters etc.
 Where data is possible to fit into pandas DataFrames, this will be preferred, but hirerachical data will be kept as json / dict structure.
 
 
 ## Example usages
 
 
+### Getting started
 ```python
 from klass import search_classification
 # Opens a ipywidget in notebooks for searching for classifications and copying code, to get started
 search_classification(no_dupes=True)
 ```
 
+### Getting a classification directly
 ```python
 from klass import get_classification # Import the utility-function
 nus = get_classification(36)
 ```
 
 ```python
 # Does the same as the code above, but does not shy away from using the class directly
 from klass import KlassClassification # Import the class for KlassClassifications
 nus = KlassClassification(36)  # Use ID for classification
+```
+
+When you have the classification stored in an object, you can "dig into" the API from there.
+```python
 codes = nus.get_codes() # codes from current date
 print(codes)
 codes.data  # Pandas dataframe available under the .data attribute
 ```
```

