# Comparing `tmp/openprotein_python-0.1.1b4.tar.gz` & `tmp/openprotein_python-0.1.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openprotein_python-0.1.1b4.tar", max compression
+gzip compressed data, was "openprotein_python-0.1.1b5.tar", max compression
```

## Comparing `openprotein_python-0.1.1b4.tar` & `openprotein_python-0.1.1b5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1543 2023-08-02 06:48:12.466765 openprotein_python-0.1.1b4/LICENSE.txt
--rw-r--r--   0        0        0     2925 2023-08-04 02:58:57.554634 openprotein_python-0.1.1b4/README.md
--rw-r--r--   0        0        0     2038 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b4/openprotein_python/__init__.py
--rw-r--r--   0        0        0      120 2023-08-03 09:03:21.855356 openprotein_python-0.1.1b4/openprotein_python/_version.py
--rw-r--r--   0        0        0      127 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b4/openprotein_python/api/__init__.py
--rw-r--r--   0        0        0    13237 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b4/openprotein_python/api/data.py
--rw-r--r--   0        0        0     8533 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b4/openprotein_python/api/design.py
--rw-r--r--   0        0        0    22209 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b4/openprotein_python/api/embedding.py
--rw-r--r--   0        0        0    14402 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b4/openprotein_python/api/jobs.py
--rw-r--r--   0        0        0    41896 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b4/openprotein_python/api/poet.py
--rw-r--r--   0        0        0    17751 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b4/openprotein_python/api/predict.py
--rw-r--r--   0        0        0    19453 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b4/openprotein_python/api/train.py
--rw-r--r--   0        0        0     3073 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b4/openprotein_python/base.py
--rw-r--r--   0        0        0      170 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b4/openprotein_python/config.py
--rw-r--r--   0        0        0     1146 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b4/openprotein_python/errors.py
--rw-r--r--   0        0        0     1055 2023-08-02 06:28:11.916350 openprotein_python-0.1.1b4/openprotein_python/fasta.py
--rw-r--r--   0        0        0     8629 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b4/openprotein_python/models.py
--rw-r--r--   0        0        0      564 2023-08-04 03:21:19.735329 openprotein_python-0.1.1b4/pyproject.toml
--rw-r--r--   0        0        0     3785 1970-01-01 00:00:00.000000 openprotein_python-0.1.1b4/PKG-INFO
+-rw-r--r--   0        0        0     1543 2023-08-02 06:48:12.466765 openprotein_python-0.1.1b5/LICENSE.txt
+-rw-r--r--   0        0        0     2925 2023-08-04 02:58:57.554634 openprotein_python-0.1.1b5/README.md
+-rw-r--r--   0        0        0     2101 2023-08-04 03:26:20.802155 openprotein_python-0.1.1b5/openprotein_python/__init__.py
+-rw-r--r--   0        0        0      120 2023-08-04 03:27:49.290985 openprotein_python-0.1.1b5/openprotein_python/_version.py
+-rw-r--r--   0        0        0      127 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b5/openprotein_python/api/__init__.py
+-rw-r--r--   0        0        0    13265 2023-08-04 03:26:28.274225 openprotein_python-0.1.1b5/openprotein_python/api/data.py
+-rw-r--r--   0        0        0     8575 2023-08-04 03:26:31.494255 openprotein_python-0.1.1b5/openprotein_python/api/design.py
+-rw-r--r--   0        0        0    22251 2023-08-04 03:26:35.154289 openprotein_python-0.1.1b5/openprotein_python/api/embedding.py
+-rw-r--r--   0        0        0    14423 2023-08-04 03:26:37.454311 openprotein_python-0.1.1b5/openprotein_python/api/jobs.py
+-rw-r--r--   0        0        0    41938 2023-08-04 03:26:41.162346 openprotein_python-0.1.1b5/openprotein_python/api/poet.py
+-rw-r--r--   0        0        0    17793 2023-08-04 03:26:54.222468 openprotein_python-0.1.1b5/openprotein_python/api/predict.py
+-rw-r--r--   0        0        0    19488 2023-08-04 03:26:57.478499 openprotein_python-0.1.1b5/openprotein_python/api/train.py
+-rw-r--r--   0        0        0     3087 2023-08-04 03:26:22.638172 openprotein_python-0.1.1b5/openprotein_python/base.py
+-rw-r--r--   0        0        0      170 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b5/openprotein_python/config.py
+-rw-r--r--   0        0        0     1146 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b5/openprotein_python/errors.py
+-rw-r--r--   0        0        0     1055 2023-08-02 06:28:11.916350 openprotein_python-0.1.1b5/openprotein_python/fasta.py
+-rw-r--r--   0        0        0     8636 2023-08-04 03:26:25.866202 openprotein_python-0.1.1b5/openprotein_python/models.py
+-rw-r--r--   0        0        0      564 2023-08-04 03:27:57.143059 openprotein_python-0.1.1b5/pyproject.toml
+-rw-r--r--   0        0        0     3785 1970-01-01 00:00:00.000000 openprotein_python-0.1.1b5/PKG-INFO
```

### Comparing `openprotein_python-0.1.1b4/LICENSE.txt` & `openprotein_python-0.1.1b5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b4/README.md` & `openprotein_python-0.1.1b5/README.md`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b4/openprotein_python/__init__.py` & `openprotein_python-0.1.1b5/openprotein_python/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from openprotein._version import __version__
+from openprotein_python._version import __version__
 
-from openprotein.base import APISession
-from openprotein.api.jobs import JobsAPI, Job
-from openprotein.api.data import DataAPI
-from openprotein.api.poet import PoetAPI
-from openprotein.api.embedding import EmbeddingAPI
-from openprotein.api.train import TrainingAPI
-from openprotein.api.design import DesignAPI
-from openprotein.api.predict import PredictAPI
+from openprotein_python.base import APISession
+from openprotein_python.api.jobs import JobsAPI, Job
+from openprotein_python.api.data import DataAPI
+from openprotein_python.api.poet import PoetAPI
+from openprotein_python.api.embedding import EmbeddingAPI
+from openprotein_python.api.train import TrainingAPI
+from openprotein_python.api.design import DesignAPI
+from openprotein_python.api.predict import PredictAPI
 class OpenProtein(APISession):
     """
     The base class for accessing OpenProtein API functionality.
     """
 
     def wait(self, job: Job, *args, **kwargs):
         return job.wait(self, *args, **kwargs)
```

### Comparing `openprotein_python-0.1.1b4/openprotein_python/api/data.py` & `openprotein_python-0.1.1b5/openprotein_python/api/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pandas as pd
 import pydantic
 from typing import Optional, List
 from io import BytesIO
 
-from openprotein.models import AssayMetadata, AssayDataPage
-from openprotein.errors import APIError
-from openprotein.base import APISession
-import openprotein.config as config
+from openprotein_python.models import AssayMetadata, AssayDataPage
+from openprotein_python.errors import APIError
+from openprotein_python.base import APISession
+import openprotein_python.config as config
 
 
 def list_models(session: APISession, assay_id: str) -> List:
     """
     List models assoicated with assay.
 
     Parameters
```

### Comparing `openprotein_python-0.1.1b4/openprotein_python/api/design.py` & `openprotein_python-0.1.1b5/openprotein_python/api/design.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Optional
 import pydantic
 
-from openprotein.base import APISession
-from openprotein.api.jobs import AsyncJobFuture, Job
-import openprotein.config as config
-from openprotein.api.jobs import load_job
-from openprotein.models import DesignJobCreate, JobType, DesignResults
-from openprotein.errors import (
+from openprotein_python.base import APISession
+from openprotein_python.api.jobs import AsyncJobFuture, Job
+import openprotein_python.config as config
+from openprotein_python.api.jobs import load_job
+from openprotein_python.models import DesignJobCreate, JobType, DesignResults
+from openprotein_python.errors import (
     APIError,
     InvalidJob,
 )
 
 def create_design_job(session: APISession, design_job: DesignJobCreate) -> Job:
     """
     Send a POST request for protein design job.
```

### Comparing `openprotein_python-0.1.1b4/openprotein_python/api/embedding.py` & `openprotein_python-0.1.1b5/openprotein_python/api/embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from openprotein.base import APISession
-from openprotein.api.jobs import (
+from openprotein_python.base import APISession
+from openprotein_python.api.jobs import (
     Job,
     MappedAsyncJobFuture,
     PagedAsyncJobFuture,
     job_get,
     JobStatus,
 )
-from openprotein.errors import InvalidJob
-import openprotein.config as config
-from openprotein.api.jobs import load_job
-from openprotein.models import (
+from openprotein_python.errors import InvalidJob
+import openprotein_python.config as config
+from openprotein_python.api.jobs import load_job
+from openprotein_python.models import (
     ModelDescription,
     TokenInfo,
     ModelMetadata,
     EmbeddedSequence,
     SVDMetadata,
     SVDJob,
     JobType,
```

### Comparing `openprotein_python-0.1.1b4/openprotein_python/api/jobs.py` & `openprotein_python-0.1.1b5/openprotein_python/api/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import time
 from enum import Enum
 
 import tqdm
 import pydantic
 from pydantic import BaseModel
 
-from openprotein.errors import TimeoutException
-from openprotein.base import APISession
-import openprotein.config as config
+from openprotein_python.errors import TimeoutException
+from openprotein_python.base import APISession
+import openprotein_python.config as config
 
 
 class JobStatus(str, Enum):
     PENDING: str = "PENDING"
     RUNNING: str = "RUNNING"
     SUCCESS: str = "SUCCESS"
     FAILURE: str = "FAILURE"
```

### Comparing `openprotein_python-0.1.1b4/openprotein_python/api/poet.py` & `openprotein_python-0.1.1b5/openprotein_python/api/poet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from typing import Optional, List, Union, BinaryIO, Iterator
 from io import BytesIO
 import random
 import csv
 import codecs
 import requests
 
-from openprotein.base import APISession
-from openprotein.api.jobs import (
+from openprotein_python.base import APISession
+from openprotein_python.api.jobs import (
     Job,
     AsyncJobFuture,
     StreamingAsyncJobFuture,
     job_get,
     job_args_get,
 )
-from openprotein.api.jobs import load_job #as base_load_job
-import openprotein.config as config
+from openprotein_python.api.jobs import load_job #as base_load_job
+import openprotein_python.config as config
 
-from openprotein.models import (
+from openprotein_python.models import (
     MSASamplingMethod,
     PoetInputType,
     PoetScoreJob,
     PoetScoreResult,
     PromptJob,
     MSAJob,
     JobType,
     PoetSSPJob,
     PoetSSPResult,
 )
-from openprotein.errors import (
+from openprotein_python.errors import (
     InvalidParameterError,
     MissingParameterError,
     APIError,
     InvalidJob,
 )
```

### Comparing `openprotein_python-0.1.1b4/openprotein_python/api/predict.py` & `openprotein_python-0.1.1b5/openprotein_python/api/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Optional, List, Union
 import pydantic
 
-from openprotein.base import APISession
-from openprotein.api.jobs import AsyncJobFuture, Job
-from openprotein.models import (
+from openprotein_python.base import APISession
+from openprotein_python.api.jobs import AsyncJobFuture, Job
+from openprotein_python.models import (
     SequenceDataset,
     SequenceData,
     PredictJob,
     PredictSingleSiteJob,
     JobType,
 )
-from openprotein.errors import InvalidParameterError, APIError, InvalidJob
-from openprotein.api.train import TrainFuture
-from openprotein.api.jobs import load_job
+from openprotein_python.errors import InvalidParameterError, APIError, InvalidJob
+from openprotein_python.api.train import TrainFuture
+from openprotein_python.api.jobs import load_job
 
 
 def _create_predict_job(
     session: APISession,
     endpoint: str,
     payload: dict,
     model_ids: Optional[List[str]] = None,
```

### Comparing `openprotein_python-0.1.1b4/openprotein_python/api/train.py` & `openprotein_python-0.1.1b5/openprotein_python/api/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional, List, Union
 import pydantic
-from openprotein.base import APISession
-from openprotein.api.jobs import AsyncJobFuture, Job
+from openprotein_python.base import APISession
+from openprotein_python.api.jobs import AsyncJobFuture, Job
 
-from openprotein.models import TrainGraph, JobType, Jobplus, CVResults
-from openprotein.errors import InvalidParameterError, APIError, InvalidJob
-from openprotein.api.data import AssayDataset, AssayMetadata
+from openprotein_python.models import TrainGraph, JobType, Jobplus, CVResults
+from openprotein_python.errors import InvalidParameterError, APIError, InvalidJob
+from openprotein_python.api.data import AssayDataset, AssayMetadata
 
 
 def list_models(session: APISession, job_id: str) -> List:
     """
     List models assoicated with job
 
     Parameters
```

### Comparing `openprotein_python-0.1.1b4/openprotein_python/base.py` & `openprotein_python-0.1.1b5/openprotein_python/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import openprotein.config as config
+import openprotein_python.config as config
 
 import requests
 from urllib.parse import urljoin
 from typing import Union
 
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 
-from openprotein.errors import APIError, InvalidParameterError, MissingParameterError, AuthError
+from openprotein_python.errors import APIError, InvalidParameterError, MissingParameterError, AuthError
 
 class BearerAuth(requests.auth.AuthBase):
     """
     See https://stackoverflow.com/a/58055668
     """
 
     def __init__(self, token):
```

### Comparing `openprotein_python-0.1.1b4/openprotein_python/errors.py` & `openprotein_python-0.1.1b5/openprotein_python/errors.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b4/openprotein_python/fasta.py` & `openprotein_python-0.1.1b5/openprotein_python/fasta.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b4/openprotein_python/models.py` & `openprotein_python-0.1.1b5/openprotein_python/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pydantic models
 from typing import Optional, List, Union, Dict, Literal
 from datetime import datetime
 from enum import Enum
 import numpy as np
 from pydantic import BaseModel, Field, validator
-from openprotein.api.jobs import Job, JobStatus
+from openprotein_python.api.jobs import Job, JobStatus
 
 class ModelDescription(BaseModel):
     citation_title: Optional[str] = None
     doi: Optional[str] = None
     summary: str
 
 class TokenInfo(BaseModel):
```

### Comparing `openprotein_python-0.1.1b4/pyproject.toml` & `openprotein_python-0.1.1b5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openprotein_python"
-version = "0.1.1b4"
+version = "0.1.1b5"
 description = "OpenProtein Python interface."
 license = "MIT"
 readme = "README.md"
 homepage = "https://docs.openprotein.ai/"
 authors = ["OpenProtein <info@ne47.bio>"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `openprotein_python-0.1.1b4/PKG-INFO` & `openprotein_python-0.1.1b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openprotein-python
-Version: 0.1.1b4
+Version: 0.1.1b5
 Summary: OpenProtein Python interface.
 Home-page: https://docs.openprotein.ai/
 License: MIT
 Author: OpenProtein
 Author-email: info@ne47.bio
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

