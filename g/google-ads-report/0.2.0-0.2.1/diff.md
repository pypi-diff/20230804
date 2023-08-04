# Comparing `tmp/google_ads_report-0.2.0.tar.gz` & `tmp/google_ads_report-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_ads_report-0.2.0.tar", max compression
+gzip compressed data, was "google_ads_report-0.2.1.tar", max compression
```

## Comparing `google_ads_report-0.2.0.tar` & `google_ads_report-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1062 2023-08-02 10:57:52.766777 google_ads_report-0.2.0/LICENSE
--rw-r--r--   0        0        0      785 2023-08-02 10:57:52.766777 google_ads_report-0.2.0/README.md
--rw-r--r--   0        0        0       81 2023-08-02 10:57:52.770777 google_ads_report-0.2.0/google_ads_report/__init__.py
--rw-r--r--   0        0        0     1110 2023-08-02 10:57:52.770777 google_ads_report-0.2.0/google_ads_report/api_client.py
--rw-r--r--   0        0        0     6091 2023-08-02 10:57:52.770777 google_ads_report-0.2.0/google_ads_report/base_client.py
--rw-r--r--   0        0        0     2593 2023-08-02 10:57:52.770777 google_ads_report-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       37 2023-08-02 10:57:52.770777 google_ads_report-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      988 2023-08-02 10:57:52.770777 google_ads_report-0.2.0/tests/test_app.py
--rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 google_ads_report-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-08-04 07:58:41.120173 google_ads_report-0.2.1/LICENSE
+-rw-r--r--   0        0        0      785 2023-08-04 07:58:41.120173 google_ads_report-0.2.1/README.md
+-rw-r--r--   0        0        0       88 2023-08-04 07:58:41.120173 google_ads_report-0.2.1/google_ads_report/__init__.py
+-rw-r--r--   0        0        0     6121 2023-08-04 07:58:41.120173 google_ads_report-0.2.1/google_ads_report/base_client.py
+-rw-r--r--   0        0        0     1486 2023-08-04 07:58:41.120173 google_ads_report-0.2.1/google_ads_report/google_ads_client.py
+-rw-r--r--   0        0        0      445 2023-08-04 07:58:41.120173 google_ads_report-0.2.1/google_ads_report/google_search_ads_client.py
+-rw-r--r--   0        0        0     2593 2023-08-04 07:58:41.120173 google_ads_report-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-08-04 07:58:41.120173 google_ads_report-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      988 2023-08-04 07:58:41.120173 google_ads_report-0.2.1/tests/test_app.py
+-rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 google_ads_report-0.2.1/PKG-INFO
```

### Comparing `google_ads_report-0.2.0/LICENSE` & `google_ads_report-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google_ads_report-0.2.0/README.md` & `google_ads_report-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `google_ads_report-0.2.0/google_ads_report/api_client.py` & `google_ads_report-0.2.1/google_ads_report/google_ads_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 
+from typing import Iterator
 from google.protobuf import json_format
 from google.ads.googleads.client import GoogleAdsClient  # type: ignore
 from .base_client import BaseClient
 
 
 class GoogleAdsApiClient(BaseClient):
     def __init__(self, credentials_path: str = None, version: str = "v14"):
@@ -15,15 +16,25 @@
         with open(credentials_path, 'r') as f:
             credentials = json.load(f)
 
         self.client = GoogleAdsClient.load_from_dict(credentials, version)
         self.ads_service = self.client.get_service("GoogleAdsService")
         self.version = version
 
-    def get_response_batch(self, customer_id, query):
+    def get_response_batch(self, customer_id: str, query: str) -> Iterator[dict]:
+        """
+        Returns a generator of batches of results from the Google Ads API.
+
+        Args:
+            customer_id: The Google Ads customer ID.
+            query: The query to run against the Google Ads API.
+
+        Returns:
+            A generator of batches of results from the Google Ads API.
+        """
         stream = self.ads_service.search_stream(customer_id=customer_id,
                                                 query=query)
         for batch in stream:
             batch_result = []
             for row in batch.results:
                 row = json_format.MessageToDict(row)
                 batch_result.append(row)
```

### Comparing `google_ads_report-0.2.0/google_ads_report/base_client.py` & `google_ads_report-0.2.1/google_ads_report/base_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Any, Dict, List, Optional, Set, Sequence
+from typing import Any, Dict, List, Optional, Set, Sequence, Iterator
 from dataclasses import dataclass
 
 import json
 
 from google.ads.googleads.client import GoogleAdsClient  # type: ignore
 from importlib import import_module
 import re
@@ -36,16 +36,16 @@
 
 class BaseClient:
 
     def __init__(self, version: str = "v14"):
         self.api_version = version
         self.google_ads_row = self._get_google_ads_row(version)
 
-    def get_response(self, entity_id: str, query_text: str):
-        pass
+    def get_response_batch(self, customer_id: str, query: str) -> Iterator[dict]:
+        ...
 
     def _get_google_ads_row(self, api_version: str) -> "GoogleAdsRow":
         base_module = f"google.ads.googleads.{api_version}"
         google_ads_service = import_module(
             f"{base_module}.services.types.google_ads_service")
         return google_ads_service.GoogleAdsRow()
```

### Comparing `google_ads_report-0.2.0/pyproject.toml` & `google_ads_report-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "google-ads-report"
-version = "0.2.0"
+version = "0.2.1"
 homepage = "https://github.com/ikameglobal/google-ads-report"
 description = "Easier to use"
 authors = ["ikameglobal <minhpc@ikameglobal.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `google_ads_report-0.2.0/tests/test_app.py` & `google_ads_report-0.2.1/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `google_ads_report-0.2.0/PKG-INFO` & `google_ads_report-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ads-report
-Version: 0.2.0
+Version: 0.2.1
 Summary: Easier to use
 Home-page: https://github.com/ikameglobal/google-ads-report
 License: MIT
 Author: ikameglobal
 Author-email: minhpc@ikameglobal.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

