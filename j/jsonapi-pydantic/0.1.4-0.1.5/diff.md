# Comparing `tmp/jsonapi-pydantic-0.1.4.tar.gz` & `tmp/jsonapi-pydantic-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonapi-pydantic-0.1.4.tar", max compression
+gzip compressed data, was "jsonapi-pydantic-0.1.5.tar", max compression
```

## Comparing `jsonapi-pydantic-0.1.4.tar` & `jsonapi-pydantic-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      101 2022-10-16 08:34:24.770203 jsonapi-pydantic-0.1.4/jsonapi_pydantic/__init__.py
--rw-r--r--   0        0        0      223 2022-10-15 16:23:47.932658 jsonapi-pydantic-0.1.4/jsonapi_pydantic/constants.py
--rw-r--r--   0        0        0      315 2022-09-13 11:40:10.663263 jsonapi-pydantic-0.1.4/jsonapi_pydantic/v1_0/__init__.py
--rw-r--r--   0        0        0     1002 2022-07-25 18:05:27.078706 jsonapi-pydantic-0.1.4/jsonapi_pydantic/v1_0/error.py
--rw-r--r--   0        0        0      314 2022-07-25 18:29:41.833025 jsonapi-pydantic-0.1.4/jsonapi_pydantic/v1_0/jsonapi.py
--rw-r--r--   0        0        0      677 2022-07-16 18:35:01.709800 jsonapi-pydantic-0.1.4/jsonapi_pydantic/v1_0/links.py
--rw-r--r--   0        0        0       73 2022-07-16 14:53:20.777589 jsonapi-pydantic-0.1.4/jsonapi_pydantic/v1_0/meta.py
--rw-r--r--   0        0        0      176 2022-07-16 14:32:16.060521 jsonapi-pydantic-0.1.4/jsonapi_pydantic/v1_0/resource/__init__.py
--rw-r--r--   0        0        0     1071 2022-07-16 17:30:50.355888 jsonapi-pydantic-0.1.4/jsonapi_pydantic/v1_0/resource/relationship.py
--rw-r--r--   0        0        0      822 2022-07-25 17:57:33.394312 jsonapi-pydantic-0.1.4/jsonapi_pydantic/v1_0/resource/relationship_links.py
--rw-r--r--   0        0        0     2040 2022-10-16 06:45:49.417347 jsonapi-pydantic-0.1.4/jsonapi_pydantic/v1_0/resource/resource.py
--rw-r--r--   0        0        0      334 2022-07-16 17:30:15.057388 jsonapi-pydantic-0.1.4/jsonapi_pydantic/v1_0/resource_identifier.py
--rw-r--r--   0        0        0     1970 2022-10-16 08:31:44.952072 jsonapi-pydantic-0.1.4/jsonapi_pydantic/v1_0/toplevel.py
--rw-r--r--   0        0        0     1097 2022-10-16 08:34:47.187535 jsonapi-pydantic-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2802 2022-07-27 18:48:54.230511 jsonapi-pydantic-0.1.4/readme.md
--rw-r--r--   0        0        0     3669 2022-10-16 08:41:48.843843 jsonapi-pydantic-0.1.4/setup.py
--rw-r--r--   0        0        0     3781 2022-10-16 08:41:48.844088 jsonapi-pydantic-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      101 2022-11-15 13:09:40.132599 jsonapi-pydantic-0.1.5/jsonapi_pydantic/__init__.py
+-rw-r--r--   0        0        0      223 2022-10-15 16:23:47.932658 jsonapi-pydantic-0.1.5/jsonapi_pydantic/constants.py
+-rw-r--r--   0        0        0      315 2022-09-13 11:40:10.663263 jsonapi-pydantic-0.1.5/jsonapi_pydantic/v1_0/__init__.py
+-rw-r--r--   0        0        0     1002 2022-07-25 18:05:27.078706 jsonapi-pydantic-0.1.5/jsonapi_pydantic/v1_0/error.py
+-rw-r--r--   0        0        0      314 2022-07-25 18:29:41.833025 jsonapi-pydantic-0.1.5/jsonapi_pydantic/v1_0/jsonapi.py
+-rw-r--r--   0        0        0      683 2022-11-15 13:06:43.375723 jsonapi-pydantic-0.1.5/jsonapi_pydantic/v1_0/links.py
+-rw-r--r--   0        0        0       73 2022-07-16 14:53:20.777589 jsonapi-pydantic-0.1.5/jsonapi_pydantic/v1_0/meta.py
+-rw-r--r--   0        0        0      176 2022-07-16 14:32:16.060521 jsonapi-pydantic-0.1.5/jsonapi_pydantic/v1_0/resource/__init__.py
+-rw-r--r--   0        0        0     1071 2022-07-16 17:30:50.355888 jsonapi-pydantic-0.1.5/jsonapi_pydantic/v1_0/resource/relationship.py
+-rw-r--r--   0        0        0      822 2022-07-25 17:57:33.394312 jsonapi-pydantic-0.1.5/jsonapi_pydantic/v1_0/resource/relationship_links.py
+-rw-r--r--   0        0        0     2040 2022-10-16 06:45:49.417347 jsonapi-pydantic-0.1.5/jsonapi_pydantic/v1_0/resource/resource.py
+-rw-r--r--   0        0        0      334 2022-07-16 17:30:15.057388 jsonapi-pydantic-0.1.5/jsonapi_pydantic/v1_0/resource_identifier.py
+-rw-r--r--   0        0        0     1970 2022-10-16 08:31:44.952072 jsonapi-pydantic-0.1.5/jsonapi_pydantic/v1_0/toplevel.py
+-rw-r--r--   0        0        0     1097 2022-11-15 13:09:35.888599 jsonapi-pydantic-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2802 2022-07-27 18:48:54.230511 jsonapi-pydantic-0.1.5/readme.md
+-rw-r--r--   0        0        0     3669 2022-11-15 13:11:55.298740 jsonapi-pydantic-0.1.5/setup.py
+-rw-r--r--   0        0        0     3781 2022-11-15 13:11:55.299006 jsonapi-pydantic-0.1.5/PKG-INFO
```

### Comparing `jsonapi-pydantic-0.1.4/jsonapi_pydantic/v1_0/error.py` & `jsonapi-pydantic-0.1.5/jsonapi_pydantic/v1_0/error.py`

 * *Files identical despite different names*

### Comparing `jsonapi-pydantic-0.1.4/jsonapi_pydantic/v1_0/links.py` & `jsonapi-pydantic-0.1.5/jsonapi_pydantic/v1_0/links.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,10 +16,10 @@
     def check_all_values(cls, values: dict) -> dict:
         # More about these restrictions: https://jsonapi.org/format/#document-links
         if len(values) < 1:
             raise ValueError("A link object can contain the following members: href, meta.")
         return values
 
 
-Links = Dict[str, Union[AnyUrl, Link]]
+Links = Dict[str, Union[AnyUrl, Link, None]]
 
 __all__ = ["Link"]
```

### Comparing `jsonapi-pydantic-0.1.4/jsonapi_pydantic/v1_0/resource/relationship.py` & `jsonapi-pydantic-0.1.5/jsonapi_pydantic/v1_0/resource/relationship.py`

 * *Files identical despite different names*

### Comparing `jsonapi-pydantic-0.1.4/jsonapi_pydantic/v1_0/resource/relationship_links.py` & `jsonapi-pydantic-0.1.5/jsonapi_pydantic/v1_0/resource/relationship_links.py`

 * *Files identical despite different names*

### Comparing `jsonapi-pydantic-0.1.4/jsonapi_pydantic/v1_0/resource/resource.py` & `jsonapi-pydantic-0.1.5/jsonapi_pydantic/v1_0/resource/resource.py`

 * *Files identical despite different names*

### Comparing `jsonapi-pydantic-0.1.4/jsonapi_pydantic/v1_0/toplevel.py` & `jsonapi-pydantic-0.1.5/jsonapi_pydantic/v1_0/toplevel.py`

 * *Files identical despite different names*

### Comparing `jsonapi-pydantic-0.1.4/pyproject.toml` & `jsonapi-pydantic-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jsonapi-pydantic"
-version = "0.1.4"
+version = "0.1.5"
 description = "JSON:API implementation with pydantic."
 
 authors = ["impocode <impocode@impocode.com>"]
 maintainers = ["impocode <impocode@impocode.com>"]
 
 license= "MIT"
 readme = "readme.md"
```

### Comparing `jsonapi-pydantic-0.1.4/readme.md` & `jsonapi-pydantic-0.1.5/readme.md`

 * *Files identical despite different names*

### Comparing `jsonapi-pydantic-0.1.4/setup.py` & `jsonapi-pydantic-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.10.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'jsonapi-pydantic',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'JSON:API implementation with pydantic.',
     'long_description': '# jsonapi-pydantic\n\n<p align="center">\n  <em><a href="https://jsonapi.org" target="_blank">JSON:API</a> implementation with <a href="https://pydantic-docs.helpmanual.io" target="_blank">Pydantic.</a>\n  </em>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/jsonapi-pydantic/" target="_blank">\n      <img src="https://img.shields.io/pypi/v/jsonapi-pydantic" alt="PyPI">\n  </a>\n  <a href="https://github.com/impocode/jsonapi-pydantic/blob/master/license.md" target="_blank">\n      <img src="https://img.shields.io/github/license/impocode/jsonapi-pydantic.svg" alt="License">\n  </a>\n</p>\n\n## Description\n\n`jsonapi-pydantic` provides a suite of Pydantic models matching the JSON:API specification.\n\n## Install\n\n```shell\n$ pip install jsonapi-pydantic\n```\n\nOr use your python package manager.\n\n## Usage\n\nObject with primary data:\n\n```python\nfrom jsonapi_pydantic.v1_0 import TopLevel\n\nexternal_data = {\n    "data": [\n        {\n            "type": "articles",\n            "id": "1",\n            "attributes": {\n                "title": "JSON:API paints my bikeshed!",\n                "body": "The shortest article. Ever.",\n                "created": "2015-05-22T14:56:29.000Z",\n                "updated": "2015-05-22T14:56:28.000Z",\n            },\n            "relationships": {"author": {"data": {"id": "42", "type": "people"}}},\n        }\n    ],\n    "included": [\n        {"type": "people", "id": "42", "attributes": {"name": "John", "age": 80, "gender": "male"}}\n    ],\n}\n\ntop_level = TopLevel(**external_data)\n\nprint(top_level.dict(exclude_unset=True))\n"""\n{\n    "data": [\n        {\n            "type": "articles",\n            "id": "1",\n            "attributes": {\n                "title": "JSON:API paints my bikeshed!",\n                "body": "The shortest article. Ever.",\n                "created": "2015-05-22T14:56:29.000Z",\n                "updated": "2015-05-22T14:56:28.000Z",\n            },\n            "relationships": {"author": {"data": {"id": "42", "type": "people"}}},\n        }\n    ],\n    "included": [\n        {"type": "people", "id": "42", "attributes": {"name": "John", "age": 80, "gender": "male"}}\n    ],\n}\n"""\nprint(top_level.data)\n"""\n[\n    Resource(\n        type="articles",\n        id="1",\n        attributes={\n            "title": "JSON:API paints my bikeshed!",\n            "body": "The shortest article. Ever.",\n            "created": "2015-05-22T14:56:29.000Z",\n            "updated": "2015-05-22T14:56:28.000Z",\n        },\n        relationships={\n            "author": Relationship(\n                links=None, data=ResourceIdentifier(id="42", type="people", meta=None), meta=None\n            )\n        },\n        links=None,\n        meta=None,\n    )\n]\n"""\n```\n\n## License\n\nSee [license.md](https://github.com/impocode/jsonapi-pydantic/blob/master/license.md).\n',
     'author': 'impocode',
     'author_email': 'impocode@impocode.com',
     'maintainer': 'impocode',
     'maintainer_email': 'impocode@impocode.com',
     'url': 'https://github.com/impocode/jsonapi-pydantic',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['jsonapi_pydantic', 'jsonapi_pydantic.v1_0', 'jsonapi_pydantic.v1_0.resource']
 package_data = \ {'': ['*']} install_requires = \ ['pydantic>=1.10.2,<2.0.0']
-setup_kwargs = { 'name': 'jsonapi-pydantic', 'version': '0.1.4', 'description':
+setup_kwargs = { 'name': 'jsonapi-pydantic', 'version': '0.1.5', 'description':
 'JSON:API implementation with pydantic.', 'long_description': '# jsonapi-
 pydantic\n\n
                  \n JSON:API implementation with Pydantic.\n\n
 \n
                        \n \n_[PyPI]\n\n \n_[License]\n\n
 \n\n## Description\n\n`jsonapi-pydantic` provides a suite of Pydantic models
 matching the JSON:API specification.\n\n## Install\n\n```shell\n$ pip install
```

### Comparing `jsonapi-pydantic-0.1.4/PKG-INFO` & `jsonapi-pydantic-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonapi-pydantic
-Version: 0.1.4
+Version: 0.1.5
 Summary: JSON:API implementation with pydantic.
 Home-page: https://github.com/impocode/jsonapi-pydantic
 License: MIT
 Keywords: jsonapi,pydantic
 Author: impocode
 Author-email: impocode@impocode.com
 Maintainer: impocode
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jsonapi-pydantic Version: 0.1.4 Summary: JSON:API
+Metadata-Version: 2.1 Name: jsonapi-pydantic Version: 0.1.5 Summary: JSON:API
 implementation with pydantic. Home-page: https://github.com/impocode/jsonapi-
 pydantic License: MIT Keywords: jsonapi,pydantic Author: impocode Author-email:
 impocode@impocode.com Maintainer: impocode Maintainer-email:
 impocode@impocode.com Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

