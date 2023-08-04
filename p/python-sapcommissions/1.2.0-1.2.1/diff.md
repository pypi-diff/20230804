# Comparing `tmp/python-sapcommissions-1.2.0.tar.gz` & `tmp/python-sapcommissions-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sapcommissions-1.2.0.tar", last modified: Thu Jul 27 12:24:39 2023, max compression
+gzip compressed data, was "python-sapcommissions-1.2.1.tar", last modified: Fri Aug  4 10:50:34 2023, max compression
```

## Comparing `python-sapcommissions-1.2.0.tar` & `python-sapcommissions-1.2.1.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/.github/workflows/pr-labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    57710 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/docs/ENDPOINTS.md
--rw-r--r--   0 runner    (1001) docker     (123)    14634 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/docs/METHODS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/python_sapcommissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-27 12:24:39.000000 python-sapcommissions-1.2.0/python_sapcommissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-27 12:24:39.000000 python-sapcommissions-1.2.0/python_sapcommissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:24:39.000000 python-sapcommissions-1.2.0/python_sapcommissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 12:24:39.000000 python-sapcommissions-1.2.0/python_sapcommissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 12:24:39.000000 python-sapcommissions-1.2.0/python_sapcommissions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/sapcommissions/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/sapcommissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58524 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/sapcommissions/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/sapcommissions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)   114107 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/sapcommissions/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/tests/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:50:34.198957 python-sapcommissions-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:50:34.194957 python-sapcommissions-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:50:34.194957 python-sapcommissions-1.2.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/.github/ISSUE_TEMPLATE/issue_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:50:34.194957 python-sapcommissions-1.2.1/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:50:34.194957 python-sapcommissions-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/.github/workflows/pr-labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:50:34.194957 python-sapcommissions-1.2.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-08-04 10:50:34.198957 python-sapcommissions-1.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:50:34.194957 python-sapcommissions-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    57719 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/docs/ENDPOINTS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14634 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/docs/METHODS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:50:34.194957 python-sapcommissions-1.2.1/python_sapcommissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-08-04 10:50:34.000000 python-sapcommissions-1.2.1/python_sapcommissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-08-04 10:50:34.000000 python-sapcommissions-1.2.1/python_sapcommissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 10:50:34.000000 python-sapcommissions-1.2.1/python_sapcommissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-04 10:50:34.000000 python-sapcommissions-1.2.1/python_sapcommissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 10:50:34.000000 python-sapcommissions-1.2.1/python_sapcommissions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:50:34.194957 python-sapcommissions-1.2.1/sapcommissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/sapcommissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58626 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/sapcommissions/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/sapcommissions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114261 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/sapcommissions/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 10:50:34.198957 python-sapcommissions-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:50:34.194957 python-sapcommissions-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/tests/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-04 10:50:26.000000 python-sapcommissions-1.2.1/tox.ini
```

### Comparing `python-sapcommissions-1.2.0/.github/scripts/release.py` & `python-sapcommissions-1.2.1/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.2.0/.github/workflows/lint.yml` & `python-sapcommissions-1.2.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.2.0/.github/workflows/publish.yml` & `python-sapcommissions-1.2.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.2.0/.pre-commit-config.yaml` & `python-sapcommissions-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.2.0/LICENSE` & `python-sapcommissions-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.2.0/PKG-INFO` & `python-sapcommissions-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sapcommissions
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python wrapper for the SAP Commissions API
 Author-email: Niels Perfors <niels.perfors1987@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/niro1987/python-sapcommissions
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
```

### Comparing `python-sapcommissions-1.2.0/docs/ENDPOINTS.md` & `python-sapcommissions-1.2.1/docs/ENDPOINTS.md`

 * *Files 1% similar despite different names*

```diff
@@ -957,16 +957,16 @@
 
 | Returns    | Description                                             |
 | ---------- | ------------------------------------------------------- |
 | `Pipeline` | `Pipeline` instance containing only the pipelineRunSeq. |
 
 <!-- Links -->
 
-[create]: README.md#create
-[create-versions]: README.md#create-versions
-[get]: README.md#get
-[get-versions]: README.md#get-versions
-[list]: README.md#list
-[update]: README.md#update
-[update-versions]: README.md#update-versions
-[delete]: README.md#delete
-[delete-versions]: README.md#delete-versions
+[create]: METHODS.md#create
+[create-versions]: METHODS.md#create-versions
+[get]: METHODS.md#get
+[get-versions]: METHODS.md#get-versions
+[list]: METHODS.md#list
+[update]: METHODS.md#update
+[update-versions]: METHODS.md#update-versions
+[delete]: METHODS.md#delete
+[delete-versions]: METHODS.md#delete-versions
```

### Comparing `python-sapcommissions-1.2.0/docs/METHODS.md` & `python-sapcommissions-1.2.1/docs/METHODS.md`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.2.0/docs/README.md` & `python-sapcommissions-1.2.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.2.0/pyproject.toml` & `python-sapcommissions-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.2.0/python_sapcommissions.egg-info/PKG-INFO` & `python-sapcommissions-1.2.1/python_sapcommissions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sapcommissions
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python wrapper for the SAP Commissions API
 Author-email: Niels Perfors <niels.perfors1987@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/niro1987/python-sapcommissions
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
```

### Comparing `python-sapcommissions-1.2.0/python_sapcommissions.egg-info/SOURCES.txt` & `python-sapcommissions-1.2.1/python_sapcommissions.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 pyproject.toml
 setup.py
 tox.ini
 .github/labeler.yml
+.github/ISSUE_TEMPLATE/config.yml
+.github/ISSUE_TEMPLATE/issue_template.yml
 .github/scripts/release.py
 .github/workflows/lint.yml
 .github/workflows/pr-labeler.yml
 .github/workflows/publish.yml
 .github/workflows/release.yml
 .vscode/settings.json
 docs/ENDPOINTS.md
```

### Comparing `python-sapcommissions-1.2.0/sapcommissions/__init__.py` & `python-sapcommissions-1.2.1/sapcommissions/__init__.py`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.2.0/sapcommissions/endpoints.py` & `python-sapcommissions-1.2.1/sapcommissions/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -836,27 +836,27 @@
 
 
 class Periods(_Create, _Delete, _Get, _List, _Update):
     resource = resources.Period
 
 
 class Pipelines(_Get, _List):  # pylint disable=too-many-public-methods
-    resource = resources.Pipeline
+    resource = resources.PipelineRun
 
     def _run_pipeline(
         self,
         stageTypeSeq: str,
         calendarSeq: str,
         periodSeq: str,
         runMode: PipelineRunMode = PipelineRunMode.FULL,
         positionSeqs: list[str] | None = None,
         removeStaleResults: bool | None = None,
         runStats: bool | None = None,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """Run a PipelineRun command."""
         command = {
             "command": "PipelineRun",
             "stageTypeSeq": stageTypeSeq,
             "calendarSeq": calendarSeq,
             "periodSeq": periodSeq,
             "runMode": runMode.value,
@@ -874,27 +874,27 @@
             command["runStats"] = runStats
         if processingUnitSeq is not None:
             command["processingUnitSeq"] = processingUnitSeq
 
         response = self._client.post(self.url, [command])
         data = response[self.name]
         pipeline_seq = data["0"][0]
-        return resources.Pipeline(pipelineRunSeq=pipeline_seq)
+        return resources.PipelineRun(pipelineRunSeq=pipeline_seq)
 
     def generate_reports(
         self,
         calendarSeq: str,
         periodSeq: str,
         formats: list[ReportFormat],
         reports: list[str],
         groups: list[str] | None = None,
         positionSeqs: list[str] | None = None,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Reports Generation pipeline.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -941,24 +941,24 @@
             command["positionSeqs"] = positionSeqs
         if processingUnitSeq is not None:
             command["processingUnitSeq"] = processingUnitSeq
 
         response = self._client.post(self.url, [command])
         data = response[self.name]
         pipeline_seq = data["0"][0]
-        return resources.Pipeline(pipelineRunSeq=pipeline_seq)
+        return resources.PipelineRun(pipelineRunSeq=pipeline_seq)
 
     def classify(
         self,
         calendarSeq: str,
         periodSeq: str,
         incremental: bool = False,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Classify pipeline.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -986,15 +986,15 @@
         self,
         calendarSeq: str,
         periodSeq: str,
         incremental: bool = False,
         positionSeqs: list[str] | None = None,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Allocate pipeline.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1024,15 +1024,15 @@
     def reward(
         self,
         calendarSeq: str,
         periodSeq: str,
         positionSeqs: list[str] | None = None,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Reward pipeline.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1056,15 +1056,15 @@
 
     def pay(
         self,
         calendarSeq: str,
         periodSeq: str,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Pay pipeline.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1085,15 +1085,15 @@
         self,
         calendarSeq: str,
         periodSeq: str,
         incremental: bool = False,
         positionSeqs: list[str] | None = None,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Summarize pipeline.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1125,15 +1125,15 @@
         calendarSeq: str,
         periodSeq: str,
         incremental: bool = False,
         positionSeqs: list[str] | None = None,
         removeStaleResults: bool = False,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Compensate pipeline.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1168,15 +1168,15 @@
         calendarSeq: str,
         periodSeq: str,
         incremental: bool = False,
         positionSeqs: list[str] | None = None,
         removeStaleResults: bool = False,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Compensate And Pay pipeline.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1208,15 +1208,15 @@
 
     def post(
         self,
         calendarSeq: str,
         periodSeq: str,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Post pipeline.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1237,15 +1237,15 @@
 
     def undo_post(
         self,
         calendarSeq: str,
         periodSeq: str,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Undo Post pipeline.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1266,15 +1266,15 @@
 
     def finalize(
         self,
         calendarSeq: str,
         periodSeq: str,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Finalize pipeline.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1295,15 +1295,15 @@
 
     def undo_finalize(
         self,
         calendarSeq: str,
         periodSeq: str,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Undo Finalize pipeline.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1324,15 +1324,15 @@
 
     def reset_from_classify(
         self,
         calendarSeq: str,
         periodSeq: str,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Reset From Classify pipeline.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1353,15 +1353,15 @@
 
     def reset_from_allocate(
         self,
         calendarSeq: str,
         periodSeq: str,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Reset From Allocate pipeline.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1382,15 +1382,15 @@
 
     def reset_from_reward(
         self,
         calendarSeq: str,
         periodSeq: str,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Reset From Reward pipeline.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1411,15 +1411,15 @@
 
     def reset_from_pay(
         self,
         calendarSeq: str,
         periodSeq: str,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Reset From Payment pipeline.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1436,15 +1436,15 @@
             periodSeq=periodSeq,
             runStats=runStats,
             processingUnitSeq=processingUnitSeq,
         )
 
     def cleanup_deferred_results(
         self, calendarSeq: str, periodSeq: str, processingUnitSeq: str | None = None
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Cleanup Deferred Results pipeline.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1458,15 +1458,15 @@
             calendarSeq=calendarSeq,
             periodSeq=periodSeq,
             processingUnitSeq=processingUnitSeq,
         )
 
     def approve_calculated_data(
         self, calendarSeq: str, periodSeq: str, processingUnitSeq: str | None = None
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Approve calculated data.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1480,15 +1480,15 @@
             calendarSeq=calendarSeq,
             periodSeq=periodSeq,
             processingUnitSeq=processingUnitSeq,
         )
 
     def purge_approved_data(
         self, calendarSeq: str, periodSeq: str, processingUnitSeq: str | None = None
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Purge approved data.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1538,15 +1538,15 @@
         stageTypeSeq: str,
         calendarSeq: str,
         batchName: str,
         runMode: ImportRunMode = ImportRunMode.ALL,
         revalidate: Revalidate | None = None,
         runStats: bool | None = None,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """Run a Import command."""
         stage_tables = _stage_tables(batchName)
         command = {
             "command": "Import",
             "stageTypeSeq": stageTypeSeq,
             "calendarSeq": calendarSeq,
             "batchName": batchName,
@@ -1560,25 +1560,25 @@
             command["runStats"] = runStats
         if processingUnitSeq is not None:
             command["processingUnitSeq"] = processingUnitSeq
 
         response = self._client.post(self.url, [command])
         data = response[self.name]
         pipeline_seq = data["0"][0]
-        return resources.Pipeline(pipelineRunSeq=pipeline_seq)
+        return resources.PipelineRun(pipelineRunSeq=pipeline_seq)
 
     def validate(
         self,
         calendarSeq: str,
         batchName: str,
         runMode: ImportRunMode = ImportRunMode.ALL,
         revalidate: Revalidate | None = None,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Validate data from stage.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1607,15 +1607,15 @@
     def transfer(
         self,
         calendarSeq: str,
         batchName: str,
         runMode: ImportRunMode = ImportRunMode.ALL,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Transfer data from stage, leave invalid data.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1640,15 +1640,15 @@
     def transfer_if_all_valid(
         self,
         calendarSeq: str,
         batchName: str,
         runMode: ImportRunMode = ImportRunMode.ALL,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Transfer data from stage only if all data is valid.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1674,15 +1674,15 @@
         self,
         calendarSeq: str,
         batchName: str,
         runMode: ImportRunMode = ImportRunMode.ALL,
         revalidate: Revalidate | None = None,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Validate and Transfer data from stage, leave invalid data.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1712,15 +1712,15 @@
         self,
         calendarSeq: str,
         batchName: str,
         runMode: ImportRunMode = ImportRunMode.ALL,
         revalidate: Revalidate | None = None,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Validate and Transfer data from stage only if all data is valid.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1749,15 +1749,15 @@
     def reset_from_validate(
         self,
         calendarSeq: str,
         periodSeq: str,
         batchName: str | None = None,
         runStats: bool = True,
         processingUnitSeq: str | None = None,
-    ) -> resources.Pipeline:
+    ) -> resources.PipelineRun:
         """
         Run Reset From Validate.
 
         Parameters
         ----------
         calendarSeq : str
             Calendar system identifier.
@@ -1779,15 +1779,15 @@
             command["batchName"] = batchName
         if processingUnitSeq is not None:
             command["processingUnitSeq"] = processingUnitSeq
 
         response = self._client.post(self.url + "/resetfromvalidate", [command])
         data = response[self.name]
         pipeline_seq = data["0"][0]
-        return resources.Pipeline(pipelineRunSeq=pipeline_seq)
+        return resources.PipelineRun(pipelineRunSeq=pipeline_seq)
 
     def purge(self, batchName: str):
         """
         Run Purge import data.
 
         Parameters
         ----------
@@ -1802,15 +1802,15 @@
             "module": stage_tables[0],
             "stageTables": stage_tables[1],
         }
 
         response = self._client.post(self.url, [command])
         data = response[self.name]
         pipeline_seq = data["0"][0]
-        return resources.Pipeline(pipelineRunSeq=pipeline_seq)
+        return resources.PipelineRun(pipelineRunSeq=pipeline_seq)
 
     def xml_import(
         self, xmlFileName: str, xmlFileContent: str, updateExistingObjects: bool = False
     ):
         """
         Run XML Import.
 
@@ -1830,15 +1830,15 @@
             "xmlFileContent": xmlFileContent,
             "updateExistingObjects": updateExistingObjects,
         }
 
         response = self._client.post(self.url, [command])
         data = response[self.name]
         pipeline_seq = data["0"][0]
-        return resources.Pipeline(pipelineRunSeq=pipeline_seq)
+        return resources.PipelineRun(pipelineRunSeq=pipeline_seq)
 
 
 class Plans(_Get, _List):
     resource = resources.Plan
 
 
 class PositionGroups(_Create, _Delete, _Get, _List, _Update):
```

### Comparing `python-sapcommissions-1.2.0/sapcommissions/resources.py` & `python-sapcommissions-1.2.1/sapcommissions/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,15 @@
     @property
     def _expands(cls) -> tuple:
         """Returns the name of the expandable attributes."""
         return tuple(
             fld.name
             for fld in fields(cls)
             if fld.type not in ("str", "int", "date", "datetime", "bool", "Value")
+            and fld.metadata.get("expand") is not False
             or fld.metadata.get("expand") is True
         )
 
     @classmethod
     def from_dict(cls, json: dict) -> _Resource:
         """Convert dictionary to _Resource instance."""
         reference_keys = ("objectType", "key", "displayName")
@@ -212,17 +213,17 @@
     appliedDepositSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     position: Position = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     earningGroupId: str = field(default=None, repr=False)
     earningCodeId: str = field(default=None, repr=False)
-    trialPipelineRun: Pipeline = field(default=None, repr=False)
+    trialPipelineRun: PipelineRun = field(default=None, repr=False)
     trialPipelineRunDate: datetime = field(default=None, repr=False)
-    postPipelineRun: Pipeline = field(default=None, repr=False)
+    postPipelineRun: PipelineRun = field(default=None, repr=False)
     postPipelineRunDate: datetime = field(default=None, repr=False)
     entryNumber: int = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
     etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
@@ -246,20 +247,20 @@
     _endpoint_name: ClassVar[str] = "balances"
     balanceSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     position: Position = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     earningGroupId: str = field(default=None, repr=False)
     earningCodeId: str = field(default=None, repr=False)
-    trialPipelineRun: Pipeline = field(default=None, repr=False)
+    trialPipelineRun: PipelineRun = field(default=None, repr=False)
     trialPipelineRunDate: datetime = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
-    applyPipelineRun: Pipeline = field(default=None, repr=False)
+    applyPipelineRun: PipelineRun = field(default=None, repr=False)
     applyPipelineRunDate: datetime = field(default=None, repr=False)
-    postPipelineRun: Pipeline = field(default=None, repr=False)
+    postPipelineRun: PipelineRun = field(default=None, repr=False)
     postPipelineRunDate: datetime = field(default=None, repr=False)
     balanceStatusId: str = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
     etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
@@ -397,15 +398,15 @@
     commissionSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     position: Position = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     incentive: Incentive = field(default=None, repr=False)
     credit: Credit = field(default=None, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
+    pipelineRun: PipelineRun = field(default=None, repr=False)
     pipelineRunDate: datetime = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
     rateValue: Value = field(default=None, repr=False)
     entryNumber: str = field(default=None, repr=False)
     businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     isPrivate: bool = field(default=None, repr=False)
     originTypeId: str = field(default=None, repr=False)
@@ -429,15 +430,15 @@
     originTypeId: str = field(default=None, repr=False)
     reason: Reason = field(default=None, repr=False)
     rule: Rule = field(default=None, repr=False)
     isRollable: bool = field(default=None, repr=False)
     rollDate: date = field(default=None, repr=False)
     isHeld: bool = field(default=None, repr=False)
     releaseDate: date = field(default=None, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
+    pipelineRun: PipelineRun = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     compensationDate: date = field(default=None, repr=False)
     comments: str = field(default=None, repr=False)
     pipelineRunDate: datetime = field(default=None, repr=False)
     isPrivate: bool = field(default=None, repr=False)
     modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     genericAttribute1: str = field(default=None, repr=False)
@@ -574,15 +575,15 @@
     originTypeId: str = field(default=None, repr=False)
     reason: Reason = field(default=None, repr=False)
     businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     rule: Rule = field(default=None, repr=False)
     depositDate: date = field(default=None, repr=False)
     isHeld: bool = field(default=None, repr=False)
     releaseDate: date = field(default=None, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
+    pipelineRun: PipelineRun = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     comments: str = field(default=None, repr=False)
     pipelineRunDate: datetime = field(default=None, repr=False)
     isPrivate: bool = field(default=None, repr=False)
     modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
@@ -879,15 +880,15 @@
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     pipelineRunDate: datetime = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     releaseDate: datetime = field(default=None, repr=False)
     businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     attainment: str = field(default=None, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
+    pipelineRun: PipelineRun = field(default=None, repr=False)
     position: Position = field(default=None, repr=False)
     rule: Rule = field(default=None, repr=False)
     isPrivate: bool = field(default=None, repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
     genericAttribute3: str = field(default=None, repr=False)
     genericAttribute4: str = field(default=None, repr=False)
@@ -1041,15 +1042,15 @@
     measurementSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     name: str = field(default=None, metadata=_meta(id=True), repr=True)
     position: Position = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     rule: Rule = field(default=None, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
+    pipelineRun: PipelineRun = field(default=None, repr=False)
     pipelineRunDate: datetime = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
     numberOfCredits: Value = field(default=None, repr=False)
     businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     isPrivate: bool = field(default=None, repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
@@ -1094,15 +1095,15 @@
     measurementSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     name: str = field(default=None, metadata=_meta(id=True), repr=True)
     position: Position = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     rule: Rule = field(default=None, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
+    pipelineRun: PipelineRun = field(default=None, repr=False)
     pipelineRunDate: datetime = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
     numberOfCredits: Value = field(default=None, repr=False)
     businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     isPrivate: bool = field(default=None, repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
@@ -1147,15 +1148,15 @@
     measurementSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     name: str = field(default=None, metadata=_meta(id=True), repr=True)
     position: Position = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     rule: Rule = field(default=None, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
+    pipelineRun: PipelineRun = field(default=None, repr=False)
     pipelineRunDate: datetime = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
     numberOfCredits: Value = field(default=None, repr=False)
     businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     isPrivate: bool = field(default=None, repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
@@ -1319,17 +1320,17 @@
     paymentSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     position: Position = field(default=None, repr=False)
     payee: Participant = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     earningGroupId: str = field(default=None, repr=False)
     earningCodeId: str = field(default=None, repr=False)
-    trialPipelineRun: Pipeline = field(default=None, repr=False)
+    trialPipelineRun: PipelineRun = field(default=None, repr=False)
     trialPipelineRunDate: datetime = field(default=None, repr=False)
-    postPipelineRun: Pipeline = field(default=None, repr=False)
+    postPipelineRun: PipelineRun = field(default=None, repr=False)
     postPipelineRunDate: datetime = field(default=None, repr=False)
     reason: str = field(default=None, repr=False)
     value: Value = field(default=None, repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
     genericAttribute3: str = field(default=None, repr=False)
     genericAttribute4: str = field(default=None, repr=False)
@@ -1386,15 +1387,15 @@
     _endpoint_name: ClassVar[str] = "paymentSummarys"
     paymentSummarySeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     position: Position = field(default=None, repr=False)
     participant: Participant = field(default=None, repr=False)
     period: Period = field(default=None, repr=False)
     earningGroupId: str = field(default=None, repr=False)
     businessUnits: list[BusinessUnit] = field(default=None, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
+    pipelineRun: PipelineRun = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     pipelineRunDate: datetime = field(default=None, repr=False)
     appliedDeposit: Value = field(default=None, repr=False)
     priorBalance: Value = field(default=None, repr=False)
     balance: Value = field(default=None, repr=False)
     payment: Value = field(default=None, repr=False)
     Deposit: Value = field(default=None, repr=False)  # pylint: disable=invalid-name
@@ -1434,15 +1435,15 @@
     )
     modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     level: int = field(default=None, repr=False)
     etag: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
 
 
 @dataclass
-class Pipeline(_Resource):
+class PipelineRun(_Resource):
     _endpoint_name: ClassVar[str] = "pipelines"
     pipelineRunSeq: int = field(default=None, metadata=_meta(seq=True), repr=False)
     batchName: str = field(default=None, repr=False)
     command: str = field(default=None, repr=False)
     dateSubmitted: datetime = field(default=None, repr=False)
     description: str = field(default=None, repr=True)
     endDateScheduled: datetime = field(default=None, repr=False)
@@ -1802,15 +1803,15 @@
     orderId: str = field(default=None, metadata=_meta(id=True), repr=True)
     businessUnits: list[BusinessUnit] = field(default=None, repr=False)
     createdBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     createDate: datetime = field(
         default=None, metadata=_meta(json_ignore=True), repr=False
     )
     modifiedBy: str = field(default=None, metadata=_meta(json_ignore=True), repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
+    pipelineRun: PipelineRun = field(default=None, repr=False)
     processingUnit: ProcessingUnit = field(default=None, repr=False)
     modelSeq: Model = field(default=None, metadata=_meta(json_ignore=True), repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
     genericAttribute3: str = field(default=None, repr=False)
     genericAttribute4: str = field(default=None, repr=False)
     genericAttribute5: str = field(default=None, repr=False)
@@ -1876,24 +1877,26 @@
     transactionAssignments: list[TransactionAssignment] = field(
         default=None, repr=False
     )
     discountType: str = field(default=None, repr=False)
     productName: str = field(default=None, repr=False)
     productDescription: str = field(default=None, repr=False)
     paymentTerms: str = field(default=None, repr=False)
-    processingUnit: ProcessingUnit = field(default=None, repr=False)
+    processingUnit: ProcessingUnit = field(
+        default=None, metadata=_meta(expand=False), repr=False
+    )
     unitValue: Value = field(default=None, repr=False)
     accountingDate: date = field(default=None, repr=False)
     discountPercent: Value = field(default=None, repr=False)
     comments: str = field(default=None, repr=False)
     productId: str = field(default=None, repr=False)
     numberOfUnits: Value = field(default=None, repr=False)
     nativeCurrencyAmount: Value = field(default=None, repr=False)
     nativeCurrency: str = field(default=None, repr=False)
-    pipelineRun: Pipeline = field(default=None, repr=False)
+    pipelineRun: PipelineRun = field(default=None, repr=False)
     alternateOrderNumber: str = field(default=None, repr=False)
     originTypeId: str = field(default=None, repr=False)
     genericAttribute1: str = field(default=None, repr=False)
     genericAttribute2: str = field(default=None, repr=False)
     genericAttribute3: str = field(default=None, repr=False)
     genericAttribute4: str = field(default=None, repr=False)
     genericAttribute5: str = field(default=None, repr=False)
```

### Comparing `python-sapcommissions-1.2.0/tests/test_base.py` & `python-sapcommissions-1.2.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.2.0/tests/test_endpoints.py` & `python-sapcommissions-1.2.1/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.2.0/tests/test_resources.py` & `python-sapcommissions-1.2.1/tests/test_resources.py`

 * *Files identical despite different names*

