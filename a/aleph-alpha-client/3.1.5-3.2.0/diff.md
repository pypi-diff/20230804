# Comparing `tmp/aleph-alpha-client-3.1.5.tar.gz` & `tmp/aleph-alpha-client-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleph-alpha-client-3.1.5.tar", last modified: Mon Jul 10 09:16:12 2023, max compression
+gzip compressed data, was "aleph-alpha-client-3.2.0.tar", last modified: Fri Aug  4 18:33:32 2023, max compression
```

## Comparing `aleph-alpha-client-3.1.5.tar` & `aleph-alpha-client-3.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:16:12.354924 aleph-alpha-client-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-10 09:16:12.354924 aleph-alpha-client-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:16:12.350924 aleph-alpha-client-3.1.5/aleph_alpha_client/
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34335 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/aleph_alpha_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/detokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/aleph_alpha_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:16:12.350924 aleph-alpha-client-3.1.5/aleph_alpha_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-10 09:16:12.000000 aleph-alpha-client-3.1.5/aleph_alpha_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-10 09:16:12.000000 aleph-alpha-client-3.1.5/aleph_alpha_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:16:12.000000 aleph-alpha-client-3.1.5/aleph_alpha_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-10 09:16:12.000000 aleph-alpha-client-3.1.5/aleph_alpha_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 09:16:12.000000 aleph-alpha-client-3.1.5/aleph_alpha_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 09:16:12.354924 aleph-alpha-client-3.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:16:12.354924 aleph-alpha-client-3.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_complete.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_detokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-10 09:16:02.000000 aleph-alpha-client-3.1.5/tests/test_wildcard_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:33:32.836073 aleph-alpha-client-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-08-04 18:33:32.836073 aleph-alpha-client-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:33:32.832073 aleph-alpha-client-3.2.0/aleph_alpha_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/aleph_alpha_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40223 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/aleph_alpha_client/aleph_alpha_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/aleph_alpha_client/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/aleph_alpha_client/detokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/aleph_alpha_client/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/aleph_alpha_client/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/aleph_alpha_client/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/aleph_alpha_client/explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/aleph_alpha_client/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/aleph_alpha_client/qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/aleph_alpha_client/summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/aleph_alpha_client/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/aleph_alpha_client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/aleph_alpha_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:33:32.832073 aleph-alpha-client-3.2.0/aleph_alpha_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-08-04 18:33:32.000000 aleph-alpha-client-3.2.0/aleph_alpha_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-04 18:33:32.000000 aleph-alpha-client-3.2.0/aleph_alpha_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 18:33:32.000000 aleph-alpha-client-3.2.0/aleph_alpha_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-04 18:33:32.000000 aleph-alpha-client-3.2.0/aleph_alpha_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-04 18:33:32.000000 aleph-alpha-client-3.2.0/aleph_alpha_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 18:33:32.836073 aleph-alpha-client-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:33:32.836073 aleph-alpha-client-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/tests/test_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/tests/test_detokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/tests/test_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/tests/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/tests/test_explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/tests/test_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/tests/test_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/tests/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-04 18:33:21.000000 aleph-alpha-client-3.2.0/tests/test_wildcard_import.py
```

### Comparing `aleph-alpha-client-3.1.5/LICENSE` & `aleph-alpha-client-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/PKG-INFO` & `aleph-alpha-client-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-alpha-client
-Version: 3.1.5
+Version: 3.2.0
 Summary: python client to interact with Aleph Alpha api endpoints
 Home-page: https://github.com/Aleph-Alpha/aleph-alpha-client
 Author: Aleph Alpha
 Author-email: support@aleph-alpha.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `aleph-alpha-client-3.1.5/README.md` & `aleph-alpha-client-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/aleph_alpha_client/__init__.py` & `aleph-alpha-client-3.2.0/aleph_alpha_client/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 )
 from .completion import CompletionRequest, CompletionResponse
 from .detokenization import DetokenizationRequest, DetokenizationResponse
 from .document import Document
 from .embedding import (
     EmbeddingRequest,
     EmbeddingResponse,
+    BatchSemanticEmbeddingRequest,
+    BatchSemanticEmbeddingResponse,
     SemanticEmbeddingRequest,
     SemanticEmbeddingResponse,
     SemanticRepresentation,
 )
 from .evaluation import EvaluationRequest, EvaluationResponse
 from .explanation import (
     CustomGranularity,
```

### Comparing `aleph-alpha-client-3.1.5/aleph_alpha_client/aleph_alpha_client.py` & `aleph-alpha-client-3.2.0/aleph_alpha_client/aleph_alpha_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from tokenizers import Tokenizer  # type: ignore
 from types import TracebackType
-from typing import Any, List, Mapping, Optional, Dict, Type, Union
+from typing import Any, List, Mapping, Optional, Dict, Type, Union, Iterator
 import aiohttp
+import asyncio
 from aiohttp_retry import RetryClient, ExponentialRetry
 import requests
 from requests import Response
 from requests.adapters import HTTPAdapter
 from requests.structures import CaseInsensitiveDict
 from urllib3.util.retry import Retry
 
@@ -22,16 +23,19 @@
 from aleph_alpha_client.evaluation import EvaluationRequest, EvaluationResponse
 from aleph_alpha_client.tokenization import TokenizationRequest, TokenizationResponse
 from aleph_alpha_client.detokenization import (
     DetokenizationRequest,
     DetokenizationResponse,
 )
 from aleph_alpha_client.embedding import (
+    BatchSemanticEmbeddingRequest,
+    BatchSemanticEmbeddingResponse,
     EmbeddingRequest,
     EmbeddingResponse,
+    EmbeddingVector,
     SemanticEmbeddingRequest,
     SemanticEmbeddingResponse,
 )
 
 POOLING_OPTIONS = ["mean", "max", "last_token", "abs_max"]
 RETRY_STATUS_CODES = frozenset({408, 429, 500, 502, 503, 504})
 DEFAULT_REQUEST_TIMEOUT = 305
@@ -66,14 +70,15 @@
 AnyRequest = Union[
     CompletionRequest,
     EmbeddingRequest,
     EvaluationRequest,
     TokenizationRequest,
     DetokenizationRequest,
     SemanticEmbeddingRequest,
+    BatchSemanticEmbeddingRequest,
     QaRequest,
     SummarizationRequest,
     ExplanationRequest,
     ExplanationRequest,
 ]
 
 
@@ -334,15 +339,15 @@
         model: str,
     ) -> SemanticEmbeddingResponse:
         """Embeds a text and returns vectors that can be used for downstream tasks
         (e.g. semantic similarity) and models (e.g. classifiers).
 
         Parameters:
             request (SemanticEmbeddingRequest, required):
-                Parameters for the requested semnatic embedding.
+                Parameters for the requested semantic embedding.
 
             model (string, required):
                 Name of model to use. A model name refers to a model architecture (number of parameters among others).
                 Always the latest version of model is used.
 
         Examples:
             >>> # function for symmetric embedding
@@ -375,14 +380,62 @@
         response = self._post_request(
             "semantic_embed",
             request,
             model,
         )
         return SemanticEmbeddingResponse.from_json(response)
 
+    def batch_semantic_embed(
+        self,
+        request: BatchSemanticEmbeddingRequest,
+        model: Optional[str] = None,
+    ) -> BatchSemanticEmbeddingResponse:
+        """Embeds a sequence of texts or images and returns vectors in the same order as they
+        were provided. If more than 100 prompts are provided then this method will chunk them
+        into batches of 100 prompts that will be sent to the API.
+
+        Parameters:
+            request (BatchSemanticEmbeddingRequest, required):
+                Parameters for the requested semantic embeddings.
+
+            model (string, optional, default None):
+                Name of model to use. A model name refers to a model architecture (number of parameters among others).
+                Always the latest version of model is used.
+
+        Examples:
+            >>> # function for symmetric embedding
+            >>> def embed_symmetric(texts: Sequence[str]):
+                    # Create an embeddingrequest with the type set to symmetric
+                    request = BatchSemanticEmbeddingRequest(
+                        prompts=[Prompt.from_text(text) for text in texts],
+                        representation=SemanticRepresentation.Symmetric
+                    )
+                    # create the embedding
+                    result = client.batch_semantic_embed(request, model=model_name)
+                    return result.embedding
+        """
+
+        responses: List[EmbeddingVector] = []
+        model_version = ""
+        # The API currently only supports batch semantic embedding requests with up to 100
+        # prompts per batch. As a convenience for users, this function chunks larger requests.
+        for batch_request in generate_semantic_embedding_batches(request):
+            raw_response = self._post_request(
+                "batch_semantic_embed",
+                batch_request,
+                model,
+            )
+            response = BatchSemanticEmbeddingResponse.from_json(raw_response)
+            model_version = response.model_version
+            responses.extend(response.embeddings)
+
+        return BatchSemanticEmbeddingResponse._from_model_version_and_embeddings(
+            model_version, responses
+        )
+
     def evaluate(
         self,
         request: EvaluationRequest,
         model: str,
     ) -> EvaluationResponse:
         """Evaluates the model's likelihood to produce a completion given a prompt.
 
@@ -776,15 +829,15 @@
         model: str,
     ) -> SemanticEmbeddingResponse:
         """Embeds a text and returns vectors that can be used for downstream tasks
         (e.g. semantic similarity) and models (e.g. classifiers).
 
         Parameters:
             request (SemanticEmbeddingRequest, required):
-                Parameters for the requested semnatic embedding.
+                Parameters for the requested semantic embedding.
 
             model (string, required):
                 Name of model to use. A model name refers to a model architecture (number of parameters among others).
                 Always the latest version of model is used.
 
         Examples:
             >>> # function for symmetric embedding
@@ -816,14 +869,70 @@
         response = await self._post_request(
             "semantic_embed",
             request,
             model,
         )
         return SemanticEmbeddingResponse.from_json(response)
 
+    async def batch_semantic_embed(
+        self,
+        request: BatchSemanticEmbeddingRequest,
+        model: Optional[str] = None,
+        num_concurrent_requests: int = 1,
+    ) -> BatchSemanticEmbeddingResponse:
+        """Embeds a sequence of texts or images and returns vectors in the same order as they
+        were provided. If more than 100 prompts are provided then this method will chunk them
+        into batches of 100 prompts that will be sent to the API.
+
+        Parameters:
+            request (BatchSemanticEmbeddingRequest, required):
+                Parameters for the requested semantic embeddings.
+
+            model (string, optional, default None):
+                Name of model to use. A model name refers to a model architecture (number of parameters among others).
+                Always the latest version of model is used.
+
+        Examples:
+            >>> # function for symmetric embedding
+            >>> def embed_symmetric(texts: Sequence[str]):
+                    # Create an embeddingrequest with the type set to symmetric
+                    request = BatchSemanticEmbeddingRequest(
+                        prompts=[Prompt.from_text(text) for text in texts],
+                        representation=SemanticRepresentation.Symmetric
+                    )
+                    # create the embedding
+                    result = client.batch_semantic_embed(request, model=model_name)
+                    return result.embedding
+        """
+        responses: List[EmbeddingVector] = []
+        model_version = ""
+
+        # The API currently only supports batch semantic embedding requests with up to 100
+        # prompts per batch. As a convenience for users, this function chunks larger requests.
+        requests = generate_semantic_embedding_batches(request)
+        results = await gather_with_concurrency(
+            num_concurrent_requests,
+            (
+                self._post_request(
+                    "batch_semantic_embed",
+                    batch_request,
+                    model,
+                )
+                for batch_request in requests
+            ),
+        )
+        for result in results:
+            resp = BatchSemanticEmbeddingResponse.from_json(result)
+            model_version = resp.model_version
+            responses.extend(resp.embeddings)
+
+        return BatchSemanticEmbeddingResponse._from_model_version_and_embeddings(
+            model_version, responses
+        )
+
     async def evaluate(
         self,
         request: EvaluationRequest,
         model: str,
     ) -> EvaluationResponse:
         """Evaluates the model's likelihood to produce a completion given a prompt.
 
@@ -921,7 +1030,37 @@
 
         Examples:
             >>> tokenizer = await client.tokenizer(model="luminous-extended")
             >>> tokenized_prompt = tokenizer.encode("Hello world")
         """
         response = await self._get_request_text(f"models/{model}/tokenizer")
         return Tokenizer.from_str(response)
+
+
+# Based on: https://docs.aleph-alpha.com/changelog/2022/11/14/async-python-client/
+async def gather_with_concurrency(n, tasks):
+    semaphore = asyncio.Semaphore(n)
+
+    async def sem_task(task):
+        async with semaphore:
+            return await task
+
+    return await asyncio.gather(*(sem_task(task) for task in tasks))
+
+
+def generate_semantic_embedding_batches(
+    request: BatchSemanticEmbeddingRequest,
+) -> List[BatchSemanticEmbeddingRequest]:
+    requests = []
+    for batch_index in range(0, len(request.prompts), 100):
+        batch = request.prompts[batch_index : batch_index + 100]
+        requests.append(
+            BatchSemanticEmbeddingRequest(
+                prompts=batch,
+                representation=request.representation,
+                compress_to_size=request.compress_to_size,
+                normalize=request.normalize,
+                contextual_control_threshold=request.contextual_control_threshold,
+                control_log_additive=request.control_log_additive,
+            )
+        )
+    return requests
```

### Comparing `aleph-alpha-client-3.1.5/aleph_alpha_client/completion.py` & `aleph-alpha-client-3.2.0/aleph_alpha_client/completion.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/aleph_alpha_client/detokenization.py` & `aleph-alpha-client-3.2.0/aleph_alpha_client/detokenization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/aleph_alpha_client/document.py` & `aleph-alpha-client-3.2.0/aleph_alpha_client/document.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/aleph_alpha_client/embedding.py` & `aleph-alpha-client-3.2.0/aleph_alpha_client/embedding.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum
 from typing import (
     Any,
     Dict,
     List,
     NamedTuple,
     Optional,
+    Sequence,
     Tuple,
 )
 from aleph_alpha_client.prompt import Prompt
 
 
 class EmbeddingRequest(NamedTuple):
     """
@@ -183,15 +184,122 @@
     def to_json(self) -> Dict[str, Any]:
         payload = self._asdict()
         payload["representation"] = self.representation.value
         payload["prompt"] = self.prompt.to_json()
         return payload
 
 
+class BatchSemanticEmbeddingRequest(NamedTuple):
+    """
+    Embeds multiple multi-modal prompts and returns their embeddings in the same order as they were supplied.
+
+    Parameters:
+        prompts
+            A list of texts and/or images to be embedded.
+        representation
+            Semantic representation to embed the prompt with.
+        compress_to_size
+            Options available: 128
+
+            The default behavior is to return the full embedding, but you can optionally request an embedding compressed to a smaller set of dimensions.
+
+            Full embedding sizes for supported models:
+              - luminous-base: 5120
+
+            The 128 size is expected to have a small drop in accuracy performance (4-6%), with the benefit of being much smaller, which makes comparing these embeddings much faster for use cases where speed is critical.
+
+            The 128 size can also perform better if you are embedding really short texts or documents.
+
+        normalize
+            Return normalized embeddings. This can be used to save on additional compute when applying a cosine similarity metric.
+
+            Note that at the moment this parameter does not yet have any effect. This will change as soon as the
+            corresponding feature is available in the backend
+
+        contextual_control_threshold (float, default None)
+            If set to None, attention control parameters only apply to those tokens that have
+            explicitly been set in the request.
+            If set to a non-None value, we apply the control parameters to similar tokens as well.
+            Controls that have been applied to one token will then be applied to all other tokens
+            that have at least the similarity score defined by this parameter.
+            The similarity score is the cosine similarity of token embeddings.
+
+        control_log_additive (bool, default True)
+            True: apply control by adding the log(control_factor) to attention scores.
+            False: apply control by (attention_scores - - attention_scores.min(-1)) * control_factor
+
+    Examples
+        >>> texts = [
+                "deep learning",
+                "artificial intelligence",
+                "deep diving",
+                "artificial snow",
+            ]
+        >>> # Texts to compare
+        >>> request = BatchSemanticEmbeddingRequest(prompts=[Prompt.from_text(text) for text in texts], representation=SemanticRepresentation.Symmetric)
+            result = model.batch_semantic_embed(request)
+    """
+
+    prompts: Sequence[Prompt]
+    representation: SemanticRepresentation
+    compress_to_size: Optional[int] = None
+    normalize: bool = False
+    contextual_control_threshold: Optional[float] = None
+    control_log_additive: Optional[bool] = True
+
+    def to_json(self) -> Dict[str, Any]:
+        payload = self._asdict()
+        payload["representation"] = self.representation.value
+        payload["prompts"] = [prompt.to_json() for prompt in self.prompts]
+        return payload
+
+
+EmbeddingVector = List[float]
+
+
 class SemanticEmbeddingResponse(NamedTuple):
+    """
+    Response of a semantic embedding request
+
+    Parameters:
+        model_version
+            Model name and version (if any) of the used model for inference
+        embedding
+            A list of floats that can be used to compare against other embeddings.
+        message
+            This field is no longer used.
+    """
+
     model_version: str
-    embedding: List[float]
+    embedding: EmbeddingVector
     message: Optional[str] = None
 
     @staticmethod
     def from_json(json: Dict[str, Any]) -> "SemanticEmbeddingResponse":
         return SemanticEmbeddingResponse(**json)
+
+
+class BatchSemanticEmbeddingResponse(NamedTuple):
+    """
+    Response of a batch semantic embedding request
+
+    Parameters:
+        model_version
+            Model name and version (if any) of the used model for inference
+        embeddings
+            A list of embeddings.
+    """
+
+    model_version: str
+    embeddings: Sequence[EmbeddingVector]
+
+    @staticmethod
+    def from_json(json: Dict[str, Any]) -> "BatchSemanticEmbeddingResponse":
+        return BatchSemanticEmbeddingResponse(**json)
+
+    @staticmethod
+    def _from_model_version_and_embeddings(
+        model_version: str, embeddings: Sequence[EmbeddingVector]
+    ) -> "BatchSemanticEmbeddingResponse":
+        return BatchSemanticEmbeddingResponse(
+            model_version=model_version, embeddings=embeddings
+        )
```

### Comparing `aleph-alpha-client-3.1.5/aleph_alpha_client/evaluation.py` & `aleph-alpha-client-3.2.0/aleph_alpha_client/evaluation.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/aleph_alpha_client/explanation.py` & `aleph-alpha-client-3.2.0/aleph_alpha_client/explanation.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/aleph_alpha_client/prompt.py` & `aleph-alpha-client-3.2.0/aleph_alpha_client/prompt.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/aleph_alpha_client/qa.py` & `aleph-alpha-client-3.2.0/aleph_alpha_client/qa.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/aleph_alpha_client/summarization.py` & `aleph-alpha-client-3.2.0/aleph_alpha_client/summarization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/aleph_alpha_client/tokenization.py` & `aleph-alpha-client-3.2.0/aleph_alpha_client/tokenization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/aleph_alpha_client.egg-info/PKG-INFO` & `aleph-alpha-client-3.2.0/aleph_alpha_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-alpha-client
-Version: 3.1.5
+Version: 3.2.0
 Summary: python client to interact with Aleph Alpha api endpoints
 Home-page: https://github.com/Aleph-Alpha/aleph-alpha-client
 Author: Aleph Alpha
 Author-email: support@aleph-alpha.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `aleph-alpha-client-3.1.5/aleph_alpha_client.egg-info/SOURCES.txt` & `aleph-alpha-client-3.2.0/aleph_alpha_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/setup.py` & `aleph-alpha-client-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/tests/test_clients.py` & `aleph-alpha-client-3.2.0/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/tests/test_complete.py` & `aleph-alpha-client-3.2.0/tests/test_complete.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/tests/test_detokenize.py` & `aleph-alpha-client-3.2.0/tests/test_detokenize.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/tests/test_embed.py` & `aleph-alpha-client-3.2.0/tests/test_embed.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 from aleph_alpha_client import EmbeddingRequest
 from aleph_alpha_client.aleph_alpha_client import AsyncClient, Client
 from aleph_alpha_client.embedding import (
+    BatchSemanticEmbeddingRequest,
     SemanticEmbeddingRequest,
     SemanticRepresentation,
 )
 from aleph_alpha_client.prompt import Prompt
 from tests.common import (
     sync_client,
     async_client,
@@ -41,20 +42,36 @@
 
     response = await async_client.semantic_embed(request, model=model_name)
     assert response.model_version is not None
     assert response.embedding
     assert len(response.embedding) == 128
 
 
+@pytest.mark.parametrize("num_prompts", [1, 100, 101, 200, 1000])
+@pytest.mark.system_test
+async def test_batch_embed_semantic_with_async_client(
+    async_client: AsyncClient, num_prompts: int
+):
+    request = BatchSemanticEmbeddingRequest(
+        prompts=[Prompt.from_text(str(i)) for i in range(num_prompts)],
+        representation=SemanticRepresentation.Symmetric,
+        compress_to_size=128,
+    )
+
+    result = await async_client.batch_semantic_embed(
+        request=request, model="luminous-base", num_concurrent_requests=10
+    )
+    assert len(result.embeddings) == num_prompts
+
+
 # Client
 
 
 @pytest.mark.system_test
 def test_embed(sync_client: Client, model_name: str):
-
     request = EmbeddingRequest(
         prompt=Prompt.from_text("hello"), layers=[0, -1], pooling=["mean", "max"]
     )
 
     result = sync_client.embed(request=request, model=model_name)
 
     assert result.model_version is not None
@@ -98,19 +115,31 @@
         request.layers
     )
     assert result.tokens is not None
 
 
 @pytest.mark.system_test
 def test_embed_semantic(sync_client: Client):
-
     request = SemanticEmbeddingRequest(
         prompt=Prompt.from_text("hello"),
         representation=SemanticRepresentation.Symmetric,
         compress_to_size=128,
     )
 
     result = sync_client.semantic_embed(request=request, model="luminous-base")
 
     assert result.model_version is not None
     assert result.embedding
     assert len(result.embedding) == 128
+
+
+@pytest.mark.parametrize("num_prompts", [1, 100, 101, 200, 1000])
+@pytest.mark.system_test
+def test_batch_embed_semantic(sync_client: Client, num_prompts: int):
+    request = BatchSemanticEmbeddingRequest(
+        prompts=[Prompt.from_text("hello") for _ in range(num_prompts)],
+        representation=SemanticRepresentation.Symmetric,
+        compress_to_size=128,
+    )
+
+    result = sync_client.batch_semantic_embed(request=request, model="luminous-base")
+    assert len(result.embeddings) == num_prompts
```

### Comparing `aleph-alpha-client-3.1.5/tests/test_error_handling.py` & `aleph-alpha-client-3.2.0/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/tests/test_evaluate.py` & `aleph-alpha-client-3.2.0/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/tests/test_explanation.py` & `aleph-alpha-client-3.2.0/tests/test_explanation.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/tests/test_image.py` & `aleph-alpha-client-3.2.0/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/tests/test_prompt.py` & `aleph-alpha-client-3.2.0/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/tests/test_qa.py` & `aleph-alpha-client-3.2.0/tests/test_qa.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/tests/test_summarize.py` & `aleph-alpha-client-3.2.0/tests/test_summarize.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.5/tests/test_tokenize.py` & `aleph-alpha-client-3.2.0/tests/test_tokenize.py`

 * *Files identical despite different names*

