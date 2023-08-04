# Comparing `tmp/connect-reports-core-26.0.0.tar.gz` & `tmp/connect_reports_core-29.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect-reports-core-26.0.0.tar", max compression
+gzip compressed data, was "connect_reports_core-29.0.tar", max compression
```

## Comparing `connect-reports-core-26.0.0.tar` & `connect_reports_core-29.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0    11357 2022-08-09 11:18:23.728308 connect-reports-core-26.0.0/LICENSE
--rw-r--r--   0        0        0     1975 2022-08-09 11:18:23.728308 connect-reports-core-26.0.0/README.md
--rw-r--r--   0        0        0       53 2022-08-09 11:18:23.728308 connect-reports-core-26.0.0/connect/reports/__init__.py
--rw-r--r--   0        0        0      184 2022-08-09 11:18:23.728308 connect-reports-core-26.0.0/connect/reports/constants.py
--rw-r--r--   0        0        0     4691 2022-08-09 11:18:23.728308 connect-reports-core-26.0.0/connect/reports/datamodels.py
--rw-r--r--   0        0        0     2240 2022-08-09 11:18:23.728308 connect-reports-core-26.0.0/connect/reports/parser.py
--rw-r--r--   0        0        0      485 2022-08-09 11:18:23.732308 connect-reports-core-26.0.0/connect/reports/renderers/__init__.py
--rw-r--r--   0        0        0     6126 2022-08-09 11:18:23.732308 connect-reports-core-26.0.0/connect/reports/renderers/base.py
--rw-r--r--   0        0        0     1368 2022-08-09 11:18:23.732308 connect-reports-core-26.0.0/connect/reports/renderers/csv.py
--rw-r--r--   0        0        0     2406 2022-08-09 11:18:23.732308 connect-reports-core-26.0.0/connect/reports/renderers/j2.py
--rw-r--r--   0        0        0     2258 2022-08-09 11:18:23.732308 connect-reports-core-26.0.0/connect/reports/renderers/json.py
--rw-r--r--   0        0        0     3320 2022-08-09 11:18:23.732308 connect-reports-core-26.0.0/connect/reports/renderers/pdf.py
--rw-r--r--   0        0        0     1031 2022-08-09 11:18:23.732308 connect-reports-core-26.0.0/connect/reports/renderers/registry.py
--rw-r--r--   0        0        0      378 2022-08-09 11:18:23.732308 connect-reports-core-26.0.0/connect/reports/renderers/utils.py
--rw-r--r--   0        0        0     5811 2022-08-09 11:18:23.732308 connect-reports-core-26.0.0/connect/reports/renderers/xlsx.py
--rw-r--r--   0        0        0     6857 2022-08-09 11:18:23.732308 connect-reports-core-26.0.0/connect/reports/schemas/reports_schema.json
--rw-r--r--   0        0        0     5227 2022-08-09 11:18:23.732308 connect-reports-core-26.0.0/connect/reports/validator.py
--rw-r--r--   0        0        0     1887 2022-08-09 11:19:51.439205 connect-reports-core-26.0.0/pyproject.toml
--rw-r--r--   0        0        0     2899 2022-08-09 11:19:52.465580 connect-reports-core-26.0.0/setup.py
--rw-r--r--   0        0        0     3146 2022-08-09 11:19:52.465967 connect-reports-core-26.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-04 08:24:01.101254 connect_reports_core-29.0/LICENSE
+-rw-r--r--   0        0        0     1975 2023-08-04 08:24:01.101254 connect_reports_core-29.0/README.md
+-rw-r--r--   0        0        0       53 2023-08-04 08:24:01.101254 connect_reports_core-29.0/connect/reports/__init__.py
+-rw-r--r--   0        0        0      184 2023-08-04 08:24:01.101254 connect_reports_core-29.0/connect/reports/constants.py
+-rw-r--r--   0        0        0     4691 2023-08-04 08:24:01.101254 connect_reports_core-29.0/connect/reports/datamodels.py
+-rw-r--r--   0        0        0     2240 2023-08-04 08:24:01.101254 connect_reports_core-29.0/connect/reports/parser.py
+-rw-r--r--   0        0        0      490 2023-08-04 08:24:01.101254 connect_reports_core-29.0/connect/reports/renderers/__init__.py
+-rw-r--r--   0        0        0     6126 2023-08-04 08:24:01.101254 connect_reports_core-29.0/connect/reports/renderers/base.py
+-rw-r--r--   0        0        0     1367 2023-08-04 08:24:01.101254 connect_reports_core-29.0/connect/reports/renderers/csv.py
+-rw-r--r--   0        0        0     2389 2023-08-04 08:24:01.101254 connect_reports_core-29.0/connect/reports/renderers/j2.py
+-rw-r--r--   0        0        0     2258 2023-08-04 08:24:01.101254 connect_reports_core-29.0/connect/reports/renderers/json.py
+-rw-r--r--   0        0        0     3320 2023-08-04 08:24:01.101254 connect_reports_core-29.0/connect/reports/renderers/pdf.py
+-rw-r--r--   0        0        0     1032 2023-08-04 08:24:01.101254 connect_reports_core-29.0/connect/reports/renderers/registry.py
+-rw-r--r--   0        0        0      378 2023-08-04 08:24:01.101254 connect_reports_core-29.0/connect/reports/renderers/utils.py
+-rw-r--r--   0        0        0     5809 2023-08-04 08:24:01.101254 connect_reports_core-29.0/connect/reports/renderers/xlsx.py
+-rw-r--r--   0        0        0     6914 2023-08-04 08:24:01.105254 connect_reports_core-29.0/connect/reports/schemas/reports_schema.json
+-rw-r--r--   0        0        0     5227 2023-08-04 08:24:01.105254 connect_reports_core-29.0/connect/reports/validator.py
+-rw-r--r--   0        0        0     2600 2023-08-04 08:24:33.485906 connect_reports_core-29.0/pyproject.toml
+-rw-r--r--   0        0        0     3178 1970-01-01 00:00:00.000000 connect_reports_core-29.0/PKG-INFO
```

### Comparing `connect-reports-core-26.0.0/LICENSE` & `connect_reports_core-29.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connect-reports-core-26.0.0/README.md` & `connect_reports_core-29.0/README.md`

 * *Files identical despite different names*

### Comparing `connect-reports-core-26.0.0/connect/reports/datamodels.py` & `connect_reports_core-29.0/connect/reports/datamodels.py`

 * *Files identical despite different names*

### Comparing `connect-reports-core-26.0.0/connect/reports/parser.py` & `connect_reports_core-29.0/connect/reports/parser.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #  Copyright © 2022 CloudBlue. All rights reserved.
 
+from connect.reports.constants import DEFAULT_RENDERER_ID
 from connect.reports.datamodels import (
     ChoicesParameterDefinition,
     ParameterDefinition,
     RendererDefinition,
     ReportDefinition,
     RepositoryDefinition,
 )
-from connect.reports.constants import DEFAULT_RENDERER_ID
 
 
 def parse(root_path, data):
     """
     Creates and returns a RepositoryDefinition object.
 
     :param root_path: Reports descriptor root path.
```

### Comparing `connect-reports-core-26.0.0/connect/reports/renderers/base.py` & `connect_reports_core-29.0/connect/reports/renderers/base.py`

 * *Files identical despite different names*

### Comparing `connect-reports-core-26.0.0/connect/reports/renderers/csv.py` & `connect_reports_core-29.0/connect/reports/renderers/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #  Copyright © 2022 CloudBlue. All rights reserved.
 
+import csv
 import inspect
 
 from connect.reports.renderers.base import BaseRenderer
 from connect.reports.renderers.registry import register
 from connect.reports.renderers.utils import aiter
 
-import csv
-
 
 @register('csv')
 class CSVRenderer(BaseRenderer):
     """
     CSV Renderer class.
     Inherits from BaseRenderer class and implements
     the generation report function, exporting the data
```

### Comparing `connect-reports-core-26.0.0/connect/reports/renderers/j2.py` & `connect_reports_core-29.0/connect/reports/renderers/j2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 #  Copyright © 2022 CloudBlue. All rights reserved.
 
 import os
 
-from jinja2 import (
-    Environment,
-    FileSystemLoader,
-    select_autoescape,
-)
+from jinja2 import Environment, FileSystemLoader, select_autoescape
 
 from connect.reports.renderers.base import BaseRenderer
 from connect.reports.renderers.registry import register
 
 
 @register('jinja2')
 class Jinja2Renderer(BaseRenderer):
```

### Comparing `connect-reports-core-26.0.0/connect/reports/renderers/json.py` & `connect_reports_core-29.0/connect/reports/renderers/json.py`

 * *Files identical despite different names*

### Comparing `connect-reports-core-26.0.0/connect/reports/renderers/pdf.py` & `connect_reports_core-29.0/connect/reports/renderers/pdf.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #  Copyright © 2022 CloudBlue. All rights reserved.
 
-import pathlib
 import os
+import pathlib
 from functools import partial
 
 from weasyprint import CSS, HTML, default_url_fetcher
 
 from connect.reports.renderers.j2 import Jinja2Renderer
 from connect.reports.renderers.registry import register
```

### Comparing `connect-reports-core-26.0.0/connect/reports/renderers/registry.py` & `connect_reports_core-29.0/connect/reports/renderers/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #  Copyright © 2022 CloudBlue. All rights reserved.
 
 from connect.reports.renderers.base import BaseRenderer
 
+
 _RENDERERS = {}
 
 
 class RendererAlreadyRegisteredError(Exception):
     pass
```

### Comparing `connect-reports-core-26.0.0/connect/reports/renderers/xlsx.py` & `connect_reports_core-29.0/connect/reports/renderers/xlsx.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 #  Copyright © 2022 CloudBlue. All rights reserved.
 
 import inspect
 import json
 import os
 from datetime import datetime
+from zipfile import BadZipfile
 
 import pytz
-
 from openpyxl import load_workbook
 from openpyxl.styles import Alignment, Font, PatternFill
-from openpyxl.styles.colors import Color, WHITE
+from openpyxl.styles.colors import WHITE, Color
 from openpyxl.utils.exceptions import InvalidFileException
 
-from zipfile import BadZipfile
-
 from connect.reports.renderers.base import BaseRenderer
 from connect.reports.renderers.registry import register
 from connect.reports.renderers.utils import aiter
 
 
 @register('xlsx')
 class XLSXRenderer(BaseRenderer):
```

### Comparing `connect-reports-core-26.0.0/connect/reports/schemas/reports_schema.json` & `connect_reports_core-29.0/connect/reports/schemas/reports_schema.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema'"}*

```diff
@@ -1,8 +1,9 @@
 {
+    "$schema": "http://json-schema.org/draft-07/schema",
     "definitions": {
         "choice": {
             "properties": {
                 "label": {
                     "description": "Choice label.",
                     "type": "string"
                 },
```

### Comparing `connect-reports-core-26.0.0/connect/reports/validator.py` & `connect_reports_core-29.0/connect/reports/validator.py`

 * *Files identical despite different names*

### Comparing `connect-reports-core-26.0.0/pyproject.toml` & `connect_reports_core-29.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "connect-reports-core"
-version = "26.0.0"
+version = "29.0"
 description = "Connect Reports Core"
 authors = ["CloudBlue LLC"]
 license = "Apache-2.0"
 packages = [
     { include = "connect" },
 ]
 readme = "./README.md"
@@ -13,45 +13,48 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Utilities",
     "Topic :: Software Development :: Libraries",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8,<4"
 openpyxl = ">=2.5.14"
 WeasyPrint = "^53.4"
 Jinja2 = ">=2,<4"
-jsonschema = "^3.2.0"
+jsonschema = ">=3,<5"
 pytz = ">=2022"
 lxml = ">=4.9"
 orjson = "^3.5.2"
-plotly = "^5.3.0"
+plotly = "5.9.0"
 kaleido = "0.2.1"
 
-[tool.poetry.dev-dependencies]
-ipython = "^7.21.0"
-pytest = "^6.1.2"
-pytest-cov = "^2.10.1"
+[tool.poetry.group.test.dependencies]
+ipython = "^8"
+pytest = ">=6.1.2,<8"
+pytest-cov = ">=2.10.1,<5"
 pytest-mock = "^3.3.1"
-coverage = {extras = ["toml"], version = "^5.3"}
-flake8 = "~3.8"
-flake8-bugbear = "~20"
+coverage = {extras = ["toml"], version = ">=5.3,<7"}
+flake8 = ">=3.8,<6"
+flake8-bugbear = ">=20,<23"
 flake8-cognitive-complexity = "^0.1"
-flake8-commas = "~2.0"
+flake8-commas = "~2.1"
 flake8-future-import = "~0.4"
-flake8-import-order = "~0.18"
-flake8-broken-line = "~0.3"
+flake8-broken-line = ">=0.3,<0.7"
+flake8-pyproject = "^1.2.2"
 fs = "^2.4.12"
-pytest-asyncio = "^0.19.0"
+pytest-asyncio = "^0.20.1"
+flake8-isort = "^6.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = "tests"
@@ -64,17 +67,45 @@
 [tool.coverage.report]
 omit = [
     "*/migrations/*",
     "*/config/*",
     "*/settings/*",
     "*/manage.py",
     "*/wsgi.py",
-    "*/urls.py"
+    "*/urls.py",
+    "*/reports/constants.py"
 ]
 
 exclude_lines = [
     "pragma: no cover",
     "def __str__",
     "def __repr__",
     "raise NotImplementedError",
     "if __name__ == .__main__.:",
 ]
+
+[tool.flake8]
+exclude = [
+    ".idea",
+    ".vscode",
+    ".git",
+    "pg_data",
+    "venv",
+    "*/settings/*.py",
+    "*/migrations/*.py"
+]
+show_source = true
+max_line_length = 100
+max_cognitive_complexity = 15
+ignore = ["FI1", "W503", "B008"]
+
+[tool.isort]
+src_paths = "*"
+sections = ["FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
+group_by_package = true
+multi_line_output = 3
+force_grid_wrap = 4
+combine_as_imports = true
+use_parentheses = true
+include_trailing_comma = true
+line_length = 100
+lines_after_imports = 2
```

### Comparing `connect-reports-core-26.0.0/setup.py` & `connect_reports_core-29.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,82 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: connect-reports-core
+Version: 29.0
+Summary: Connect Reports Core
+Home-page: https://connect.cloudblue.com
+License: Apache-2.0
+Author: CloudBlue LLC
+Requires-Python: >=3.8,<4
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Utilities
+Requires-Dist: Jinja2 (>=2,<4)
+Requires-Dist: WeasyPrint (>=53.4,<54.0)
+Requires-Dist: jsonschema (>=3,<5)
+Requires-Dist: kaleido (==0.2.1)
+Requires-Dist: lxml (>=4.9)
+Requires-Dist: openpyxl (>=2.5.14)
+Requires-Dist: orjson (>=3.5.2,<4.0.0)
+Requires-Dist: plotly (==5.9.0)
+Requires-Dist: pytz (>=2022)
+Project-URL: Repository, https://github.com/cloudblue/connect-reports-core
+Description-Content-Type: text/markdown
+
+# Connect Reports Core
+
+![pyversions](https://img.shields.io/pypi/pyversions/connect-reports-core.svg) [![PyPi Status](https://img.shields.io/pypi/v/connect-reports-core.svg)](https://pypi.org/project/connect-reports-core/) [![Build Connect Reports Core](https://github.com/cloudblue/connect-reports-core/actions/workflows/build.yml/badge.svg)](https://github.com/cloudblue/connect-reports-core/actions/workflows/build.yml) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=connect-reports-core&metric=alert_status)](https://sonarcloud.io/dashboard?id=connect-reports-core) [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=connect-reports-core&metric=coverage)](https://sonarcloud.io/dashboard?id=connect-reports-core) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=connect-reports-core&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=connect-reports-core)
+
+## Introduction
+
+`Connect Reports Core` is the kernel package for handling reports on CloudBlue Connect Ecosystem. 
+This library is reponsible for validation of reports definition, choosing of renderer for parsing process and writing results of reports execution.
+
+
+## Install
+
+`Connect Reports Core` requires python 3.8 or later and has the following dependencies:
+
+* openpyxl>=2.5.14
+* WeasyPrint>=53.4
+* Jinja2>=2.11.3
+* jsonschema<=3.2.0
+* pytz>=2021.1
+* lxml>=4.7.1
+
+`Connect Reports Core` can be installed from [pypi.org](https://pypi.org/project/connect-reports-core/) using pip:
+
+```
+$ pip install connect-reports-core
+```
+
+## Testing
+
+On MacOs:
+* Install system dependencies
+```commandline
+brew install py3cairo pango
+```
+* Create virtualenv
+* Install project dependencies
+```commandline
+pip install poetry
+poetry update
+```
+* Run tests
+```commandline
+poetry run pytest
+```
 
-packages = \
-['connect', 'connect.reports', 'connect.reports.renderers']
 
-package_data = \
-{'': ['*'], 'connect.reports': ['schemas/*']}
+## License
 
-install_requires = \
-['Jinja2>=2,<4',
- 'WeasyPrint>=53.4,<54.0',
- 'jsonschema>=3.2.0,<4.0.0',
- 'kaleido==0.2.1',
- 'lxml>=4.9',
- 'openpyxl>=2.5.14',
- 'orjson>=3.5.2,<4.0.0',
- 'plotly>=5.3.0,<6.0.0',
- 'pytz>=2022']
-
-setup_kwargs = {
-    'name': 'connect-reports-core',
-    'version': '26.0.0',
-    'description': 'Connect Reports Core',
-    'long_description': '# Connect Reports Core\n\n![pyversions](https://img.shields.io/pypi/pyversions/connect-reports-core.svg) [![PyPi Status](https://img.shields.io/pypi/v/connect-reports-core.svg)](https://pypi.org/project/connect-reports-core/) [![Build Connect Reports Core](https://github.com/cloudblue/connect-reports-core/actions/workflows/build.yml/badge.svg)](https://github.com/cloudblue/connect-reports-core/actions/workflows/build.yml) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=connect-reports-core&metric=alert_status)](https://sonarcloud.io/dashboard?id=connect-reports-core) [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=connect-reports-core&metric=coverage)](https://sonarcloud.io/dashboard?id=connect-reports-core) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=connect-reports-core&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=connect-reports-core)\n\n## Introduction\n\n`Connect Reports Core` is the kernel package for handling reports on CloudBlue Connect Ecosystem. \nThis library is reponsible for validation of reports definition, choosing of renderer for parsing process and writing results of reports execution.\n\n\n## Install\n\n`Connect Reports Core` requires python 3.8 or later and has the following dependencies:\n\n* openpyxl>=2.5.14\n* WeasyPrint>=53.4\n* Jinja2>=2.11.3\n* jsonschema<=3.2.0\n* pytz>=2021.1\n* lxml>=4.7.1\n\n`Connect Reports Core` can be installed from [pypi.org](https://pypi.org/project/connect-reports-core/) using pip:\n\n```\n$ pip install connect-reports-core\n```\n\n## Testing\n\nOn MacOs:\n* Install system dependencies\n```commandline\nbrew install py3cairo pango\n```\n* Create virtualenv\n* Install project dependencies\n```commandline\npip install poetry\npoetry update\n```\n* Run tests\n```commandline\npoetry run pytest\n```\n\n\n## License\n\n``Connect Reports Core`` is released under the [Apache License Version 2.0](https://www.apache.org/licenses/LICENSE-2.0).\n',
-    'author': 'CloudBlue LLC',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://connect.cloudblue.com',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+``Connect Reports Core`` is released under the [Apache License Version 2.0](https://www.apache.org/licenses/LICENSE-2.0).
 
-
-setup(**setup_kwargs)
```

