# Comparing `tmp/cybrex-1.2.2.tar.gz` & `tmp/cybrex-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.2.2.tar", last modified: Wed Aug  2 15:02:37 2023, max compression
+gzip compressed data, was "cybrex-1.2.3.tar", last modified: Fri Aug  4 07:30:49 2023, max compression
```

## Comparing `cybrex-1.2.2.tar` & `cybrex-1.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-02 15:02:37.327445 cybrex-1.2.2/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.2.2/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-02 15:02:37.326851 cybrex-1.2.2/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.2.2/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-02 15:02:37.322362 cybrex-1.2.2/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.2.2/cybrex/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     5682 2023-08-02 10:33:10.000000 cybrex-1.2.2/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)    12869 2023-08-02 15:02:09.000000 cybrex-1.2.2/cybrex/cybrex_ai.py
--rw-r--r--   0 pasha      (501) staff       (20)    13592 2023-08-02 15:01:57.000000 cybrex-1.2.2/cybrex/models.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-02 15:02:37.326293 cybrex-1.2.2/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-02 15:02:37.000000 cybrex-1.2.2/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      305 2023-08-02 15:02:37.000000 cybrex-1.2.2/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-02 15:02:37.000000 cybrex-1.2.2/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-02 15:02:37.000000 cybrex-1.2.2/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-02 15:02:37.000000 cybrex-1.2.2/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-02 15:02:37.000000 cybrex-1.2.2/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-02 15:02:21.000000 cybrex-1.2.2/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-02 11:17:07.000000 cybrex-1.2.2/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-02 15:02:37.327668 cybrex-1.2.2/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-04 07:30:49.219799 cybrex-1.2.3/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.2.3/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-04 07:30:49.219147 cybrex-1.2.3/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.2.3/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-04 07:30:49.215266 cybrex-1.2.3/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.2.3/cybrex/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5649 2023-08-04 07:30:23.000000 cybrex-1.2.3/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    13015 2023-08-04 07:30:23.000000 cybrex-1.2.3/cybrex/cybrex_ai.py
+-rw-r--r--   0 pasha      (501) staff       (20)    13715 2023-08-03 17:15:53.000000 cybrex-1.2.3/cybrex/models.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-04 07:30:49.218603 cybrex-1.2.3/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-04 07:30:49.000000 cybrex-1.2.3/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      305 2023-08-04 07:30:49.000000 cybrex-1.2.3/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-04 07:30:49.000000 cybrex-1.2.3/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-04 07:30:49.000000 cybrex-1.2.3/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-04 07:30:49.000000 cybrex-1.2.3/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-04 07:30:49.000000 cybrex-1.2.3/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-04 07:30:23.000000 cybrex-1.2.3/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-02 11:17:07.000000 cybrex-1.2.3/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-04 07:30:49.219931 cybrex-1.2.3/setup.cfg
```

### Comparing `cybrex-1.2.2/PKG-INFO` & `cybrex-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.2.2
+Version: 1.2.3
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.2.2/README.md` & `cybrex-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.2.2/cybrex/cli.py` & `cybrex-1.2.3/cybrex/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,18 +42,15 @@
 
     async def import_texts(self, input_path: str):
         """
         Import binary file with embeddings
 
         :param input_path:
         """
-        async with self.cybrex as cybrex:
-            await cybrex.import_texts(
-                input_path=input_path,
-            )
+        await self.cybrex.import_texts(input_path=input_path)
 
     async def chat_doc(self, field: str, value: str, question: str, n_results: int = 4):
         """
         Ask a question about content of document identified by DOI.
 
         :param field: name of the field in document used for selection
         :param value: value of the field in document used for selection
@@ -63,15 +60,20 @@
         """
         async with self.cybrex as cybrex:
             print(f"{colored('Document', 'green')}: {field}:{value}")
             print(f"{colored('Q', 'green')}: {question}")
             response = await cybrex.chat_document(field, value, question, n_results)
             print(f"{colored('A', 'green')}: {response}")
 
-    async def chat_sci(self, query: str, n_results: int = 4, n_summa_documents: int = 10):
+    async def chat_sci(
+        self,
+        query: str,
+        n_results: int = 4,
+        n_summa_documents: int = 10,
+    ):
         """
         Ask a question about content of document identified by DOI.
 
         :param query: Text question to the document
         :param n_results: the number of documents to extract from Chroma
             more means more tokens to use and more precision in answer
         :param n_summa_documents: the number of documents to extract from Chroma
```

### Comparing `cybrex-1.2.2/cybrex/cybrex_ai.py` & `cybrex-1.2.3/cybrex/cybrex_ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         self.model = CybrexModel(config['model'])
 
         self.db = chromadb.PersistentClient(path=os.path.join(self.home_path, 'chroma'))
         self.collection_name = self.model.get_embeddings_id()
 
         self.collection = self.db.get_or_create_collection(
             name=self.collection_name,
-            embedding_function=self.model.embedder.embed_documents,
+            embedding_function=self.model.embed_documents,
         )
         self.geck = geck
         if not self.geck:
             self.geck = StcGeck(
                 ipfs_http_base_url=config['ipfs']['http']['base_url'],
                 grpc_api_endpoint=config['summa']['endpoint']
             )
@@ -252,28 +252,28 @@
         result = await asyncio.get_running_loop().run_in_executor(
             None,
             lambda: self.model.llm.ask_documents(query, documents),
         )
 
         return result
 
-    async def chat_science(self, query: str, n_results: int, n_summa_documents: int):
+    async def chat_science(self, query: str, n_results: int, n_summa_documents: int, semantic_threshold: float = 0.5):
         full_documents = await self.keywords_search(query, n_summa_documents)
 
         await self.add_full_documents(full_documents)
 
-        documents = await self._query(query, n_results)
+        documents = await self._query(query, n_results, semantic_threshold=semantic_threshold)
         answer = await asyncio.get_running_loop().run_in_executor(
             None,
             lambda: self.model.llm.ask_documents(query, documents),
         )
 
         return answer, documents, await self.get_summa_documents_from_documents(documents)
 
-    async def _query(self, query: str, n_results: int = 3, where: Optional[dict] = None):
+    async def _query(self, query: str, n_results: int = 3, where: Optional[dict] = None, semantic_threshold: float = 0.5):
         logging.getLogger('statbox').info({
             'action': 'query',
             'query': query,
             'n_results': n_results,
             'where': where,
         })
         response = await asyncio.get_running_loop().run_in_executor(
@@ -283,15 +283,16 @@
                 n_results=n_results,
                 include=['documents', 'metadatas', 'distances'],
                 where=where,
             )
         )
         documents = []
         for (text, metadata, distance) in zip(response['documents'][0], response['metadatas'][0], response['distances'][0]):
-            documents.append({'text': text, 'metadata': metadata, 'distance': distance})
+            if distance < semantic_threshold:
+                documents.append({'text': text, 'metadata': metadata, 'distance': distance})
         return documents
 
     async def keywords_search(self, query: str, n_summa_documents: int):
         if not n_summa_documents:
             return []
         logging.getLogger('statbox').info({
             'action': 'extract_keywords',
```

### Comparing `cybrex-1.2.2/cybrex/models.py` & `cybrex-1.2.3/cybrex/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,17 @@
                 query_instruction="Represent science question for retrieval",
             )
         elif self.config['embedder']['model_type'] == 'openai':
             return OpenAIEmbeddings(model=self.config['embedder']['model_name'])
         else:
             raise ValueError("Unsupported embedding model")
 
+    def embed_documents(self, texts: List[str]) -> List[List[float]]:
+        return self.embedder.embed_documents(texts)
+
     @lazy
     def llm(self):
         if self.config['llm']['model_type'] == 'llama':
             return LLM(
                 llm=AutoModelForCausalLM.from_pretrained(**self.config['llm']['config']),
                 prompter=BasePrompter.prompter_from_type(self.config['llm']['prompter']['type'])
             )
```

### Comparing `cybrex-1.2.2/cybrex.egg-info/PKG-INFO` & `cybrex-1.2.3/cybrex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.2.2
+Version: 1.2.3
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.2.2/pyproject.toml` & `cybrex-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.2.2"
+version = "1.2.3"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

