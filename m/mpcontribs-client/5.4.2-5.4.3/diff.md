# Comparing `tmp/mpcontribs-client-5.4.2.tar.gz` & `tmp/mpcontribs-client-5.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpcontribs-client-5.4.2.tar", last modified: Thu Jul  6 21:52:37 2023, max compression
+gzip compressed data, was "mpcontribs-client-5.4.3.tar", last modified: Fri Aug  4 19:38:21 2023, max compression
```

## Comparing `mpcontribs-client-5.4.2.tar` & `mpcontribs-client-5.4.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:52:37.341100 mpcontribs-client-5.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-06 21:52:37.341100 mpcontribs-client-5.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:52:37.337099 mpcontribs-client-5.4.2/mpcontribs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:52:37.337099 mpcontribs-client-5.4.2/mpcontribs/client/
--rw-r--r--   0 runner    (1001) docker     (123)    87020 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/mpcontribs/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:52:37.337099 mpcontribs-client-5.4.2/mpcontribs_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-06 21:52:36.000000 mpcontribs-client-5.4.2/mpcontribs_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-06 21:52:37.000000 mpcontribs-client-5.4.2/mpcontribs_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:52:36.000000 mpcontribs-client-5.4.2/mpcontribs_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:52:36.000000 mpcontribs-client-5.4.2/mpcontribs_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-06 21:52:36.000000 mpcontribs-client-5.4.2/mpcontribs_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 21:52:36.000000 mpcontribs-client-5.4.2/mpcontribs_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:52:37.341100 mpcontribs-client-5.4.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:52:37.341100 mpcontribs-client-5.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:52:37.341100 mpcontribs-client-5.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-06 21:52:25.000000 mpcontribs-client-5.4.2/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:21.349626 mpcontribs-client-5.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-08-04 19:38:21.349626 mpcontribs-client-5.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:21.345625 mpcontribs-client-5.4.3/mpcontribs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:21.345625 mpcontribs-client-5.4.3/mpcontribs/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    87188 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/mpcontribs/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:21.345625 mpcontribs-client-5.4.3/mpcontribs_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-08-04 19:38:20.000000 mpcontribs-client-5.4.3/mpcontribs_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-04 19:38:21.000000 mpcontribs-client-5.4.3/mpcontribs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:38:20.000000 mpcontribs-client-5.4.3/mpcontribs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:38:20.000000 mpcontribs-client-5.4.3/mpcontribs_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-04 19:38:20.000000 mpcontribs-client-5.4.3/mpcontribs_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 19:38:20.000000 mpcontribs-client-5.4.3/mpcontribs_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:21.349626 mpcontribs-client-5.4.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 19:38:21.349626 mpcontribs-client-5.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:38:21.349626 mpcontribs-client-5.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-08-04 19:38:09.000000 mpcontribs-client-5.4.3/tests/test_client.py
```

### Comparing `mpcontribs-client-5.4.2/LICENSE` & `mpcontribs-client-5.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.2/PKG-INFO` & `mpcontribs-client-5.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.4.2
+Version: 5.4.3
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.4.2/README.md` & `mpcontribs-client-5.4.3/README.md`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.2/mpcontribs/client/__init__.py` & `mpcontribs-client-5.4.3/mpcontribs/client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import plotly.io as pio
 import itertools
 import functools
 import requests
 import logging
 import datetime
 
+from inspect import getfullargspec
 from math import isclose
 from semantic_version import Version
 from requests.exceptions import RequestException
 from bravado_core.param import Param
 from bson.objectid import ObjectId
 from typing import Union, Type, List
 from tqdm.auto import tqdm
@@ -51,14 +52,15 @@
 from filetype.types.archive import Gz
 from filetype.types.image import Jpeg, Png, Gif, Tiff
 from pint import UnitRegistry
 from pint.unit import UnitDefinition
 from pint.converters import ScaleConverter
 from pint.errors import DimensionalityError
 from tempfile import gettempdir
+from plotly.express._chart_types import line as line_chart
 
 RETRIES = 3
 MAX_WORKERS = 3
 MAX_ELEMS = 10
 MAX_NESTING = 5
 MEGABYTES = 1024 * 1024
 MAX_BYTES = 2.4 * MEGABYTES
@@ -303,16 +305,17 @@
 
 class Table(pd.DataFrame):
     """Wrapper class around pandas.DataFrame to provide display() and info()"""
     def display(self):
         """Display a plotly graph for the table if in IPython/Jupyter"""
         if _in_ipython():
             try:
-                # TODO make sure that attrs only contains valid kwargs
-                return self.plot(**self.attrs)
+                allowed_kwargs = getfullargspec(line_chart).args
+                attrs = {k: v for k, v in self.attrs.items() if k in allowed_kwargs}
+                return self.plot(**attrs)
             except Exception as e:
                 logger.error(f"Can't display table: {e}")
 
         return self
 
     def info(self) -> Type[Dict]:
         """Show summary info for table"""
```

### Comparing `mpcontribs-client-5.4.2/mpcontribs_client.egg-info/PKG-INFO` & `mpcontribs-client-5.4.3/mpcontribs_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.4.2
+Version: 5.4.3
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.4.2/mpcontribs_client.egg-info/SOURCES.txt` & `mpcontribs-client-5.4.3/mpcontribs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.2/requirements/deployment.txt` & `mpcontribs-client-5.4.3/requirements/deployment.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,86 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=MPContribs/mpcontribs-client/requirements/deployment.txt --resolver=backtracking MPContribs/mpcontribs-client/setup.py python/requirements.txt
+#    pip-compile --output-file=MPContribs/mpcontribs-client/requirements/deployment.txt MPContribs/mpcontribs-client/setup.py python/requirements.txt
 #
-annotated-types==0.5.0
-    # via pydantic
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
-    # via jsonschema
+    # via
+    #   jsonschema
+    #   referencing
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 bravado==11.0.3
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-bravado-core==5.17.1
+bravado-core==6.1.0
     # via bravado
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 contourpy==1.1.0
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.3.0
+dnspython==2.4.1
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.58.0
+emmet-core==0.63.1
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-fonttools==4.40.0
+fonttools==4.42.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-frozendict==2.3.8
-    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 ipython==8.14.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 isoduration==20.11.0
     # via jsonschema
-jedi==0.18.2
+jedi==0.19.0
     # via ipython
+joblib==1.3.1
+    # via pymatgen
 json2html==1.3.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
-jsonschema[format]==4.17.3
+jsonschema[format]==4.18.6
     # via
     #   bravado-core
     #   swagger-spec-validator
+jsonschema-specifications==2023.7.1
+    # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-matplotlib==3.7.1
+matplotlib==3.7.2
     # via
     #   -r python/requirements.txt
     #   pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 monotonic==1.6
     # via bravado
@@ -128,73 +130,79 @@
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 plotly==5.15.0
     # via
     #   mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
     #   pymatgen
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pydantic==2.0
-    # via emmet-core
-pydantic-core==2.0.1
-    # via pydantic
+pydantic==1.10.12
+    # via
+    #   emmet-core
+    #   pymatgen
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-pymatgen==2023.6.28
+pymatgen==2023.7.20
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-pymongo==4.4.0
+pymongo==4.4.1
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-pyparsing==3.1.0
+pyparsing==3.0.9
     # via matplotlib
-pyrsistent==0.19.3
-    # via jsonschema
 python-dateutil==2.8.2
     # via
     #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
     #   pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
+referencing==0.30.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
+rpds-py==0.9.2
+    # via
+    #   jsonschema
+    #   referencing
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.11.1
     # via
     #   -r python/requirements.txt
@@ -241,23 +249,22 @@
     #   matplotlib-inline
 typing-extensions==4.7.1
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
-    #   pydantic-core
     #   swagger-spec-validator
 ujson==5.8.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.3
+urllib3==2.0.4
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `mpcontribs-client-5.4.2/requirements/macos-latest_py3.10.txt` & `mpcontribs-client-5.4.3/requirements/ubuntu-latest_py3.8.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,84 +1,91 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.10.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt
 #
-appnope==0.1.3
-    # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
-    # via jsonschema
+    # via
+    #   jsonschema
+    #   referencing
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
-bravado-core==5.17.1
+bravado-core==6.1.0
     # via bravado
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 contourpy==1.1.0
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.3.0
+dnspython==2.4.1
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.57.2
+emmet-core==0.63.1
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.40.0
+fonttools==4.42.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-frozendict==2.3.8
-    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
-ipython==8.14.0
+importlib-resources==6.0.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+    #   matplotlib
+ipython==8.12.2
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
-jedi==0.18.2
+jedi==0.19.0
     # via ipython
+joblib==1.3.1
+    # via pymatgen
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
 jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
-jsonschema[format]==4.17.3
+jsonschema[format]==4.18.5
     # via
     #   bravado-core
     #   swagger-spec-validator
+jsonschema-specifications==2023.7.1
+    # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-matplotlib==3.7.1
+matplotlib==3.7.2
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
@@ -92,15 +99,15 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.25.0
+numpy==1.24.4
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
@@ -116,84 +123,94 @@
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.5.0
+pillow==10.0.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
 plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pydantic==1.10.9
-    # via emmet-core
+pydantic==1.10.12
+    # via
+    #   emmet-core
+    #   pymatgen
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.6.28
+pymatgen==2023.7.20
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.4.0
+pymongo==4.4.1
     # via mpcontribs-client (setup.py)
-pyparsing==3.1.0
+pyparsing==3.0.9
     # via matplotlib
-pyrsistent==0.19.3
-    # via jsonschema
 python-dateutil==2.8.2
     # via
     #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
     #   pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
+referencing==0.30.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
+rpds-py==0.9.2
+    # via
+    #   jsonschema
+    #   referencing
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
-scipy==1.11.1
+scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
 simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
@@ -227,31 +244,34 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.7.0
+typing-extensions==4.7.1
     # via
     #   bravado
     #   emmet-core
+    #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
 ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.3
+urllib3==2.0.4
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
+zipp==3.16.2
+    # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `mpcontribs-client-5.4.2/requirements/macos-latest_py3.10_extras.txt` & `mpcontribs-client-5.4.3/requirements/macos-latest_py3.10_extras.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,94 +1,98 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt
 #
 appnope==0.1.3
     # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
-    # via jsonschema
+    # via
+    #   jsonschema
+    #   referencing
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
-bravado-core==5.17.1
+bravado-core==6.1.0
     # via bravado
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.3.0
+dnspython==2.4.1
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.57.2
+emmet-core==0.63.1
     # via mp-api
-exceptiongroup==1.1.1
+exceptiongroup==1.1.2
     # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
-flake8==6.0.0
+flake8==6.1.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.40.0
+fonttools==4.42.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-frozendict==2.3.8
-    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 iniconfig==2.0.0
     # via pytest
 ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
-jedi==0.18.2
+jedi==0.19.0
     # via ipython
+joblib==1.3.1
+    # via pymatgen
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
 jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
-jsonschema[format]==4.17.3
+jsonschema[format]==4.18.5
     # via
     #   bravado-core
     #   swagger-spec-validator
+jsonschema-specifications==2023.7.1
+    # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-matplotlib==3.7.1
+matplotlib==3.7.2
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 mccabe==0.7.0
     # via flake8
 monotonic==1.6
     # via bravado
@@ -104,15 +108,15 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.25.0
+numpy==1.25.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
@@ -129,61 +133,61 @@
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.5.0
+pillow==10.0.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
 plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 pluggy==1.2.0
     # via pytest
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 py==1.11.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-pycodestyle
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pycodestyle==2.10.0
+pycodestyle==2.11.0
     # via
     #   flake8
     #   pytest-pycodestyle
-pydantic==1.10.9
-    # via emmet-core
-pyflakes==3.0.1
+pydantic==1.10.12
+    # via
+    #   emmet-core
+    #   pymatgen
+pyflakes==3.1.0
     # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.6.28
+pymatgen==2023.7.20
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.4.0
+pymongo==4.4.1
     # via mpcontribs-client (setup.py)
-pyparsing==3.1.0
+pyparsing==3.0.9
     # via matplotlib
-pyrsistent==0.19.3
-    # via jsonschema
 pytest==7.4.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
 pytest-cov==4.1.0
@@ -199,33 +203,41 @@
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
     #   pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
+referencing==0.30.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
+rpds-py==0.9.2
+    # via
+    #   jsonschema
+    #   referencing
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.11.1
     # via pymatgen
 semantic-version==2.10.0
@@ -268,30 +280,30 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.7.0
+typing-extensions==4.7.1
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
 ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.3
+urllib3==2.0.4
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `mpcontribs-client-5.4.2/requirements/macos-latest_py3.8.txt` & `mpcontribs-client-5.4.3/requirements/macos-latest_py3.8_extras.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,108 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.8.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt
 #
 appnope==0.1.3
     # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
-    # via jsonschema
+    # via
+    #   jsonschema
+    #   referencing
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
-bravado-core==5.17.1
+bravado-core==6.1.0
     # via bravado
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 contourpy==1.1.0
     # via matplotlib
+coverage[toml]==7.2.7
+    # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.3.0
+dnspython==2.4.1
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.57.2
+emmet-core==0.63.1
     # via mp-api
+exceptiongroup==1.1.2
+    # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
+flake8==6.1.0
+    # via
+    #   mpcontribs-client (setup.py)
+    #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.40.0
+fonttools==4.42.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-frozendict==2.3.8
-    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
-importlib-resources==5.12.0
+importlib-resources==6.0.0
     # via
     #   jsonschema
+    #   jsonschema-specifications
     #   matplotlib
+iniconfig==2.0.0
+    # via pytest
 ipython==8.12.2
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
-jedi==0.18.2
+jedi==0.19.0
     # via ipython
+joblib==1.3.1
+    # via pymatgen
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
 jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
-jsonschema[format]==4.17.3
+jsonschema[format]==4.18.5
     # via
     #   bravado-core
     #   swagger-spec-validator
+jsonschema-specifications==2023.7.1
+    # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-matplotlib==3.7.1
+matplotlib==3.7.2
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
+mccabe==0.7.0
+    # via flake8
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
@@ -108,93 +125,126 @@
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
+    #   pytest
 palettable==3.3.3
     # via pymatgen
 pandas==2.0.3
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.5.0
+pillow==10.0.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
 pkgutil-resolve-name==1.3.10
     # via jsonschema
 plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-prompt-toolkit==3.0.38
+pluggy==1.2.0
+    # via pytest
+prompt-toolkit==3.0.39
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
+py==1.11.0
+    # via
+    #   mpcontribs-client (setup.py)
+    #   pytest-pycodestyle
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pydantic==1.10.9
-    # via emmet-core
+pycodestyle==2.11.0
+    # via
+    #   flake8
+    #   pytest-pycodestyle
+pydantic==1.10.12
+    # via
+    #   emmet-core
+    #   pymatgen
+pyflakes==3.1.0
+    # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.6.28
+pymatgen==2023.7.20
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.4.0
+pymongo==4.4.1
     # via mpcontribs-client (setup.py)
-pyparsing==3.1.0
+pyparsing==3.0.9
     # via matplotlib
-pyrsistent==0.19.3
-    # via jsonschema
+pytest==7.4.0
+    # via
+    #   mpcontribs-client (setup.py)
+    #   pytest-cov
+    #   pytest-flake8
+    #   pytest-pycodestyle
+pytest-cov==4.1.0
+    # via mpcontribs-client (setup.py)
+pytest-flake8==1.1.1
+    # via mpcontribs-client (setup.py)
+pytest-pycodestyle==2.3.1
+    # via mpcontribs-client (setup.py)
 python-dateutil==2.8.2
     # via
     #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
     #   pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
+referencing==0.30.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
+rpds-py==0.9.2
+    # via
+    #   jsonschema
+    #   referencing
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
@@ -225,23 +275,27 @@
     #   mpcontribs-client (setup.py)
 sympy==1.12
     # via pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
     # via plotly
+tomli==2.0.1
+    # via
+    #   coverage
+    #   pytest
 tqdm==4.65.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.7.0
+typing-extensions==4.7.1
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
@@ -249,18 +303,18 @@
     # via pandas
 ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.3
+urllib3==2.0.4
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
-zipp==3.15.0
+zipp==3.16.2
     # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `mpcontribs-client-5.4.2/requirements/macos-latest_py3.8_extras.txt` & `mpcontribs-client-5.4.3/requirements/macos-latest_py3.9_extras.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,98 +1,100 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt
 #
 appnope==0.1.3
     # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
-    # via jsonschema
+    # via
+    #   jsonschema
+    #   referencing
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
-bravado-core==5.17.1
+bravado-core==6.1.0
     # via bravado
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.3.0
+dnspython==2.4.1
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.57.2
+emmet-core==0.63.1
     # via mp-api
-exceptiongroup==1.1.1
+exceptiongroup==1.1.2
     # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
-flake8==6.0.0
+flake8==6.1.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.40.0
+fonttools==4.42.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-frozendict==2.3.8
-    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
-importlib-resources==5.12.0
-    # via
-    #   jsonschema
-    #   matplotlib
+importlib-resources==6.0.0
+    # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipython==8.12.2
+ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
-jedi==0.18.2
+jedi==0.19.0
     # via ipython
+joblib==1.3.1
+    # via pymatgen
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
 jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
-jsonschema[format]==4.17.3
+jsonschema[format]==4.18.5
     # via
     #   bravado-core
     #   swagger-spec-validator
+jsonschema-specifications==2023.7.1
+    # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-matplotlib==3.7.1
+matplotlib==3.7.2
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 mccabe==0.7.0
     # via flake8
 monotonic==1.6
     # via bravado
@@ -108,15 +110,15 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.4
+numpy==1.25.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
@@ -133,63 +135,61 @@
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.5.0
+pillow==10.0.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
 plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 pluggy==1.2.0
     # via pytest
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 py==1.11.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-pycodestyle
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pycodestyle==2.10.0
+pycodestyle==2.11.0
     # via
     #   flake8
     #   pytest-pycodestyle
-pydantic==1.10.9
-    # via emmet-core
-pyflakes==3.0.1
+pydantic==1.10.12
+    # via
+    #   emmet-core
+    #   pymatgen
+pyflakes==3.1.0
     # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.6.28
+pymatgen==2023.7.20
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.4.0
+pymongo==4.4.1
     # via mpcontribs-client (setup.py)
-pyparsing==3.1.0
+pyparsing==3.0.9
     # via matplotlib
-pyrsistent==0.19.3
-    # via jsonschema
 pytest==7.4.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
 pytest-cov==4.1.0
@@ -205,38 +205,46 @@
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
     #   pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
+referencing==0.30.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
+rpds-py==0.9.2
+    # via
+    #   jsonschema
+    #   referencing
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
-scipy==1.10.1
+scipy==1.11.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
 simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
@@ -274,15 +282,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.7.0
+typing-extensions==4.7.1
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
@@ -290,18 +298,18 @@
     # via pandas
 ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.3
+urllib3==2.0.4
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
-zipp==3.15.0
+zipp==3.16.2
     # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `mpcontribs-client-5.4.2/requirements/macos-latest_py3.9.txt` & `mpcontribs-client-5.4.3/requirements/macos-latest_py3.8.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,93 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.9.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.8.txt
 #
 appnope==0.1.3
     # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
-    # via jsonschema
+    # via
+    #   jsonschema
+    #   referencing
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
-bravado-core==5.17.1
+bravado-core==6.1.0
     # via bravado
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 contourpy==1.1.0
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.3.0
+dnspython==2.4.1
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.57.2
+emmet-core==0.63.1
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.40.0
+fonttools==4.42.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-frozendict==2.3.8
-    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
-importlib-resources==5.12.0
-    # via matplotlib
-ipython==8.14.0
+importlib-resources==6.0.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+    #   matplotlib
+ipython==8.12.2
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
-jedi==0.18.2
+jedi==0.19.0
     # via ipython
+joblib==1.3.1
+    # via pymatgen
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
 jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
-jsonschema[format]==4.17.3
+jsonschema[format]==4.18.5
     # via
     #   bravado-core
     #   swagger-spec-validator
+jsonschema-specifications==2023.7.1
+    # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-matplotlib==3.7.1
+matplotlib==3.7.2
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
@@ -94,15 +101,15 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.25.0
+numpy==1.24.4
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
@@ -118,84 +125,94 @@
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.5.0
+pillow==10.0.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
 plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pydantic==1.10.9
-    # via emmet-core
+pydantic==1.10.12
+    # via
+    #   emmet-core
+    #   pymatgen
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.6.28
+pymatgen==2023.7.20
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.4.0
+pymongo==4.4.1
     # via mpcontribs-client (setup.py)
-pyparsing==3.1.0
+pyparsing==3.0.9
     # via matplotlib
-pyrsistent==0.19.3
-    # via jsonschema
 python-dateutil==2.8.2
     # via
     #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
     #   pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
+referencing==0.30.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
+rpds-py==0.9.2
+    # via
+    #   jsonschema
+    #   referencing
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
-scipy==1.11.1
+scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
 simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
@@ -229,15 +246,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.7.0
+typing-extensions==4.7.1
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
@@ -245,18 +262,18 @@
     # via pandas
 ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.3
+urllib3==2.0.4
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
-zipp==3.15.0
+zipp==3.16.2
     # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `mpcontribs-client-5.4.2/requirements/macos-latest_py3.9_extras.txt` & `mpcontribs-client-5.4.3/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,96 +1,98 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt
 #
-appnope==0.1.3
-    # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
-    # via jsonschema
+    # via
+    #   jsonschema
+    #   referencing
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
-bravado-core==5.17.1
+bravado-core==6.1.0
     # via bravado
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.3.0
+dnspython==2.4.1
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.57.2
+emmet-core==0.63.1
     # via mp-api
-exceptiongroup==1.1.1
+exceptiongroup==1.1.2
     # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
-flake8==6.0.0
+flake8==6.1.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.40.0
+fonttools==4.42.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-frozendict==2.3.8
-    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
-importlib-resources==5.12.0
+importlib-resources==6.0.0
     # via matplotlib
 iniconfig==2.0.0
     # via pytest
 ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
-jedi==0.18.2
+jedi==0.19.0
     # via ipython
+joblib==1.3.1
+    # via pymatgen
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
 jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
-jsonschema[format]==4.17.3
+jsonschema[format]==4.18.5
     # via
     #   bravado-core
     #   swagger-spec-validator
+jsonschema-specifications==2023.7.1
+    # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-matplotlib==3.7.1
+matplotlib==3.7.2
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 mccabe==0.7.0
     # via flake8
 monotonic==1.6
     # via bravado
@@ -106,15 +108,15 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.25.0
+numpy==1.25.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
@@ -131,61 +133,61 @@
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.5.0
+pillow==10.0.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
 plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 pluggy==1.2.0
     # via pytest
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 py==1.11.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-pycodestyle
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pycodestyle==2.10.0
+pycodestyle==2.11.0
     # via
     #   flake8
     #   pytest-pycodestyle
-pydantic==1.10.9
-    # via emmet-core
-pyflakes==3.0.1
+pydantic==1.10.12
+    # via
+    #   emmet-core
+    #   pymatgen
+pyflakes==3.1.0
     # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.6.28
+pymatgen==2023.7.20
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.4.0
+pymongo==4.4.1
     # via mpcontribs-client (setup.py)
-pyparsing==3.1.0
+pyparsing==3.0.9
     # via matplotlib
-pyrsistent==0.19.3
-    # via jsonschema
 pytest==7.4.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
 pytest-cov==4.1.0
@@ -201,33 +203,41 @@
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
     #   pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
+referencing==0.30.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
+rpds-py==0.9.2
+    # via
+    #   jsonschema
+    #   referencing
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.11.1
     # via pymatgen
 semantic-version==2.10.0
@@ -270,15 +280,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.7.0
+typing-extensions==4.7.1
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
@@ -286,18 +296,18 @@
     # via pandas
 ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.3
+urllib3==2.0.4
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
-zipp==3.15.0
+zipp==3.16.2
     # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.10.txt` & `mpcontribs-client-5.4.3/requirements/macos-latest_py3.10.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,82 +1,88 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.10.txt
 #
+appnope==0.1.3
+    # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
-    # via jsonschema
+    # via
+    #   jsonschema
+    #   referencing
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
-bravado-core==5.17.1
+bravado-core==6.1.0
     # via bravado
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 contourpy==1.1.0
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.3.0
+dnspython==2.4.1
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.57.2
+emmet-core==0.63.1
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.40.0
+fonttools==4.42.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-frozendict==2.3.8
-    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
-jedi==0.18.2
+jedi==0.19.0
     # via ipython
+joblib==1.3.1
+    # via pymatgen
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
 jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
-jsonschema[format]==4.17.3
+jsonschema[format]==4.18.5
     # via
     #   bravado-core
     #   swagger-spec-validator
+jsonschema-specifications==2023.7.1
+    # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-matplotlib==3.7.1
+matplotlib==3.7.2
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
@@ -90,15 +96,15 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.25.0
+numpy==1.25.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
@@ -114,79 +120,87 @@
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.5.0
+pillow==10.0.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
 plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pydantic==1.10.9
-    # via emmet-core
+pydantic==1.10.12
+    # via
+    #   emmet-core
+    #   pymatgen
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.6.28
+pymatgen==2023.7.20
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.4.0
+pymongo==4.4.1
     # via mpcontribs-client (setup.py)
-pyparsing==3.1.0
+pyparsing==3.0.9
     # via matplotlib
-pyrsistent==0.19.3
-    # via jsonschema
 python-dateutil==2.8.2
     # via
     #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
     #   pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
+referencing==0.30.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
+rpds-py==0.9.2
+    # via
+    #   jsonschema
+    #   referencing
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.11.1
     # via pymatgen
 semantic-version==2.10.0
@@ -225,30 +239,30 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.7.0
+typing-extensions==4.7.1
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
 ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.3
+urllib3==2.0.4
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.10_extras.txt` & `mpcontribs-client-5.4.3/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,92 +1,96 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt
 #
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
-    # via jsonschema
+    # via
+    #   jsonschema
+    #   referencing
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
-bravado-core==5.17.1
+bravado-core==6.1.0
     # via bravado
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 contourpy==1.1.0
     # via matplotlib
 coverage[toml]==7.2.7
     # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.3.0
+dnspython==2.4.1
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.57.2
+emmet-core==0.63.1
     # via mp-api
-exceptiongroup==1.1.1
+exceptiongroup==1.1.2
     # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
-flake8==6.0.0
+flake8==6.1.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.40.0
+fonttools==4.42.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-frozendict==2.3.8
-    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 iniconfig==2.0.0
     # via pytest
 ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
-jedi==0.18.2
+jedi==0.19.0
     # via ipython
+joblib==1.3.1
+    # via pymatgen
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
 jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
-jsonschema[format]==4.17.3
+jsonschema[format]==4.18.5
     # via
     #   bravado-core
     #   swagger-spec-validator
+jsonschema-specifications==2023.7.1
+    # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-matplotlib==3.7.1
+matplotlib==3.7.2
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 mccabe==0.7.0
     # via flake8
 monotonic==1.6
     # via bravado
@@ -102,15 +106,15 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.25.0
+numpy==1.25.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
@@ -127,61 +131,61 @@
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.5.0
+pillow==10.0.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
 plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 pluggy==1.2.0
     # via pytest
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 py==1.11.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-pycodestyle
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pycodestyle==2.10.0
+pycodestyle==2.11.0
     # via
     #   flake8
     #   pytest-pycodestyle
-pydantic==1.10.9
-    # via emmet-core
-pyflakes==3.0.1
+pydantic==1.10.12
+    # via
+    #   emmet-core
+    #   pymatgen
+pyflakes==3.1.0
     # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.6.28
+pymatgen==2023.7.20
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.4.0
+pymongo==4.4.1
     # via mpcontribs-client (setup.py)
-pyparsing==3.1.0
+pyparsing==3.0.9
     # via matplotlib
-pyrsistent==0.19.3
-    # via jsonschema
 pytest==7.4.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
 pytest-cov==4.1.0
@@ -197,33 +201,41 @@
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
     #   pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
+referencing==0.30.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
+rpds-py==0.9.2
+    # via
+    #   jsonschema
+    #   referencing
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.11.1
     # via pymatgen
 semantic-version==2.10.0
@@ -266,30 +278,30 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.7.0
+typing-extensions==4.7.1
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
 ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.3
+urllib3==2.0.4
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.8.txt` & `mpcontribs-client-5.4.3/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,89 +1,106 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt
 #
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
-    # via jsonschema
+    # via
+    #   jsonschema
+    #   referencing
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
-bravado-core==5.17.1
+bravado-core==6.1.0
     # via bravado
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 contourpy==1.1.0
     # via matplotlib
+coverage[toml]==7.2.7
+    # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.3.0
+dnspython==2.4.1
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.57.2
+emmet-core==0.63.1
     # via mp-api
+exceptiongroup==1.1.2
+    # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
+flake8==6.1.0
+    # via
+    #   mpcontribs-client (setup.py)
+    #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.40.0
+fonttools==4.42.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-frozendict==2.3.8
-    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
-importlib-resources==5.12.0
+importlib-resources==6.0.0
     # via
     #   jsonschema
+    #   jsonschema-specifications
     #   matplotlib
+iniconfig==2.0.0
+    # via pytest
 ipython==8.12.2
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
-jedi==0.18.2
+jedi==0.19.0
     # via ipython
+joblib==1.3.1
+    # via pymatgen
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
 jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
-jsonschema[format]==4.17.3
+jsonschema[format]==4.18.5
     # via
     #   bravado-core
     #   swagger-spec-validator
+jsonschema-specifications==2023.7.1
+    # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-matplotlib==3.7.1
+matplotlib==3.7.2
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
+mccabe==0.7.0
+    # via flake8
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
@@ -106,93 +123,126 @@
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
+    #   pytest
 palettable==3.3.3
     # via pymatgen
 pandas==2.0.3
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.5.0
+pillow==10.0.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
 pkgutil-resolve-name==1.3.10
     # via jsonschema
 plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-prompt-toolkit==3.0.38
+pluggy==1.2.0
+    # via pytest
+prompt-toolkit==3.0.39
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
+py==1.11.0
+    # via
+    #   mpcontribs-client (setup.py)
+    #   pytest-pycodestyle
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pydantic==1.10.9
-    # via emmet-core
+pycodestyle==2.11.0
+    # via
+    #   flake8
+    #   pytest-pycodestyle
+pydantic==1.10.12
+    # via
+    #   emmet-core
+    #   pymatgen
+pyflakes==3.1.0
+    # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.6.28
+pymatgen==2023.7.20
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.4.0
+pymongo==4.4.1
     # via mpcontribs-client (setup.py)
-pyparsing==3.1.0
+pyparsing==3.0.9
     # via matplotlib
-pyrsistent==0.19.3
-    # via jsonschema
+pytest==7.4.0
+    # via
+    #   mpcontribs-client (setup.py)
+    #   pytest-cov
+    #   pytest-flake8
+    #   pytest-pycodestyle
+pytest-cov==4.1.0
+    # via mpcontribs-client (setup.py)
+pytest-flake8==1.1.1
+    # via mpcontribs-client (setup.py)
+pytest-pycodestyle==2.3.1
+    # via mpcontribs-client (setup.py)
 python-dateutil==2.8.2
     # via
     #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
     #   pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
+referencing==0.30.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
+rpds-py==0.9.2
+    # via
+    #   jsonschema
+    #   referencing
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
@@ -223,23 +273,27 @@
     #   mpcontribs-client (setup.py)
 sympy==1.12
     # via pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
     # via plotly
+tomli==2.0.1
+    # via
+    #   coverage
+    #   pytest
 tqdm==4.65.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.7.0
+typing-extensions==4.7.1
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
@@ -247,18 +301,18 @@
     # via pandas
 ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.3
+urllib3==2.0.4
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
-zipp==3.15.0
+zipp==3.16.2
     # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.8_extras.txt` & `mpcontribs-client-5.4.3/requirements/ubuntu-latest_py3.9.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,91 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt
 #
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
-    # via jsonschema
+    # via
+    #   jsonschema
+    #   referencing
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
-bravado-core==5.17.1
+bravado-core==6.1.0
     # via bravado
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 contourpy==1.1.0
     # via matplotlib
-coverage[toml]==7.2.7
-    # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.3.0
+dnspython==2.4.1
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.57.2
+emmet-core==0.63.1
     # via mp-api
-exceptiongroup==1.1.1
-    # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
-flake8==6.0.0
-    # via
-    #   mpcontribs-client (setup.py)
-    #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.40.0
+fonttools==4.42.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-frozendict==2.3.8
-    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
-importlib-resources==5.12.0
-    # via
-    #   jsonschema
-    #   matplotlib
-iniconfig==2.0.0
-    # via pytest
-ipython==8.12.2
+importlib-resources==6.0.0
+    # via matplotlib
+ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
-jedi==0.18.2
+jedi==0.19.0
     # via ipython
+joblib==1.3.1
+    # via pymatgen
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
 jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
-jsonschema[format]==4.17.3
+jsonschema[format]==4.18.5
     # via
     #   bravado-core
     #   swagger-spec-validator
+jsonschema-specifications==2023.7.1
+    # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-matplotlib==3.7.1
+matplotlib==3.7.2
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
-mccabe==0.7.0
-    # via flake8
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
@@ -106,135 +96,116 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.4
+numpy==1.25.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
-    #   pytest
 palettable==3.3.3
     # via pymatgen
 pandas==2.0.3
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.5.0
+pillow==10.0.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
 plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-pluggy==1.2.0
-    # via pytest
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py==1.11.0
-    # via
-    #   mpcontribs-client (setup.py)
-    #   pytest-pycodestyle
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pycodestyle==2.10.0
+pydantic==1.10.12
     # via
-    #   flake8
-    #   pytest-pycodestyle
-pydantic==1.10.9
-    # via emmet-core
-pyflakes==3.0.1
-    # via flake8
+    #   emmet-core
+    #   pymatgen
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.6.28
+pymatgen==2023.7.20
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.4.0
+pymongo==4.4.1
     # via mpcontribs-client (setup.py)
-pyparsing==3.1.0
+pyparsing==3.0.9
     # via matplotlib
-pyrsistent==0.19.3
-    # via jsonschema
-pytest==7.4.0
-    # via
-    #   mpcontribs-client (setup.py)
-    #   pytest-cov
-    #   pytest-flake8
-    #   pytest-pycodestyle
-pytest-cov==4.1.0
-    # via mpcontribs-client (setup.py)
-pytest-flake8==1.1.1
-    # via mpcontribs-client (setup.py)
-pytest-pycodestyle==2.3.1
-    # via mpcontribs-client (setup.py)
 python-dateutil==2.8.2
     # via
     #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
     #   pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
+referencing==0.30.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
+rpds-py==0.9.2
+    # via
+    #   jsonschema
+    #   referencing
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
-scipy==1.10.1
+scipy==1.11.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
 simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
@@ -260,27 +231,23 @@
     #   mpcontribs-client (setup.py)
 sympy==1.12
     # via pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
     # via plotly
-tomli==2.0.1
-    # via
-    #   coverage
-    #   pytest
 tqdm==4.65.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.7.0
+typing-extensions==4.7.1
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
@@ -288,18 +255,18 @@
     # via pandas
 ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.3
+urllib3==2.0.4
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
-zipp==3.15.0
+zipp==3.16.2
     # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.9.txt` & `mpcontribs-client-5.4.3/requirements/macos-latest_py3.9.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,90 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.9.txt
 #
+appnope==0.1.3
+    # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
-    # via jsonschema
+    # via
+    #   jsonschema
+    #   referencing
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
-bravado-core==5.17.1
+bravado-core==6.1.0
     # via bravado
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 contourpy==1.1.0
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.3.0
+dnspython==2.4.1
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.57.2
+emmet-core==0.63.1
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.40.0
+fonttools==4.42.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-frozendict==2.3.8
-    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
-importlib-resources==5.12.0
+importlib-resources==6.0.0
     # via matplotlib
 ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
-jedi==0.18.2
+jedi==0.19.0
     # via ipython
+joblib==1.3.1
+    # via pymatgen
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
 jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
-jsonschema[format]==4.17.3
+jsonschema[format]==4.18.5
     # via
     #   bravado-core
     #   swagger-spec-validator
+jsonschema-specifications==2023.7.1
+    # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-matplotlib==3.7.1
+matplotlib==3.7.2
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
@@ -92,15 +98,15 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.25.0
+numpy==1.25.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
@@ -116,79 +122,87 @@
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.5.0
+pillow==10.0.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
 plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pydantic==1.10.9
-    # via emmet-core
+pydantic==1.10.12
+    # via
+    #   emmet-core
+    #   pymatgen
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.6.28
+pymatgen==2023.7.20
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.4.0
+pymongo==4.4.1
     # via mpcontribs-client (setup.py)
-pyparsing==3.1.0
+pyparsing==3.0.9
     # via matplotlib
-pyrsistent==0.19.3
-    # via jsonschema
 python-dateutil==2.8.2
     # via
     #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
     #   pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
+referencing==0.30.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
+rpds-py==0.9.2
+    # via
+    #   jsonschema
+    #   referencing
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.11.1
     # via pymatgen
 semantic-version==2.10.0
@@ -227,15 +241,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.7.0
+typing-extensions==4.7.1
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
@@ -243,18 +257,18 @@
     # via pandas
 ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.3
+urllib3==2.0.4
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
-zipp==3.15.0
+zipp==3.16.2
     # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `mpcontribs-client-5.4.2/requirements/ubuntu-latest_py3.9_extras.txt` & `mpcontribs-client-5.4.3/requirements/ubuntu-latest_py3.10.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,99 +1,89 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt
 #
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
-    # via jsonschema
+    # via
+    #   jsonschema
+    #   referencing
 backcall==0.2.0
     # via ipython
 boltons==23.0.0
     # via mpcontribs-client (setup.py)
 bravado==11.0.3
     # via mpcontribs-client (setup.py)
-bravado-core==5.17.1
+bravado-core==6.1.0
     # via bravado
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 contourpy==1.1.0
     # via matplotlib
-coverage[toml]==7.2.7
-    # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
-dnspython==2.3.0
+dnspython==2.4.1
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.57.2
+emmet-core==0.63.1
     # via mp-api
-exceptiongroup==1.1.1
-    # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
-flake8==6.0.0
-    # via
-    #   mpcontribs-client (setup.py)
-    #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.40.0
+fonttools==4.42.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
-frozendict==2.3.8
-    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
-importlib-resources==5.12.0
-    # via matplotlib
-iniconfig==2.0.0
-    # via pytest
 ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
-jedi==0.18.2
+jedi==0.19.0
     # via ipython
+joblib==1.3.1
+    # via pymatgen
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
 jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
-jsonschema[format]==4.17.3
+jsonschema[format]==4.18.5
     # via
     #   bravado-core
     #   swagger-spec-validator
+jsonschema-specifications==2023.7.1
+    # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-matplotlib==3.7.1
+matplotlib==3.7.2
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
-mccabe==0.7.0
-    # via flake8
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
@@ -104,128 +94,111 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.25.0
+numpy==1.25.2
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
-    #   pytest
 palettable==3.3.3
     # via pymatgen
 pandas==2.0.3
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==9.5.0
+pillow==10.0.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
 plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-pluggy==1.2.0
-    # via pytest
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.39
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py==1.11.0
-    # via
-    #   mpcontribs-client (setup.py)
-    #   pytest-pycodestyle
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pycodestyle==2.10.0
+pydantic==1.10.12
     # via
-    #   flake8
-    #   pytest-pycodestyle
-pydantic==1.10.9
-    # via emmet-core
-pyflakes==3.0.1
-    # via flake8
+    #   emmet-core
+    #   pymatgen
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.6.28
+pymatgen==2023.7.20
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.4.0
+pymongo==4.4.1
     # via mpcontribs-client (setup.py)
-pyparsing==3.1.0
+pyparsing==3.0.9
     # via matplotlib
-pyrsistent==0.19.3
-    # via jsonschema
-pytest==7.4.0
-    # via
-    #   mpcontribs-client (setup.py)
-    #   pytest-cov
-    #   pytest-flake8
-    #   pytest-pycodestyle
-pytest-cov==4.1.0
-    # via mpcontribs-client (setup.py)
-pytest-flake8==1.1.1
-    # via mpcontribs-client (setup.py)
-pytest-pycodestyle==2.3.1
-    # via mpcontribs-client (setup.py)
 python-dateutil==2.8.2
     # via
     #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
 pytz==2023.3
     # via
     #   bravado-core
     #   pandas
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   bravado
     #   bravado-core
     #   pybtex
     #   swagger-spec-validator
+referencing==0.30.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
 requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
+rpds-py==0.9.2
+    # via
+    #   jsonschema
+    #   referencing
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.11.1
     # via pymatgen
 semantic-version==2.10.0
@@ -256,46 +229,39 @@
     #   mpcontribs-client (setup.py)
 sympy==1.12
     # via pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
     # via plotly
-tomli==2.0.1
-    # via
-    #   coverage
-    #   pytest
 tqdm==4.65.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.7.0
+typing-extensions==4.7.1
     # via
     #   bravado
     #   emmet-core
-    #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
 ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.3
+urllib3==2.0.4
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
-zipp==3.15.0
-    # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `mpcontribs-client-5.4.2/setup.py` & `mpcontribs-client-5.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.2/tests/test_client.py` & `mpcontribs-client-5.4.3/tests/test_client.py`

 * *Files identical despite different names*

