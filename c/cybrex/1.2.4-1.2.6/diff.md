# Comparing `tmp/cybrex-1.2.4.tar.gz` & `tmp/cybrex-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.2.4.tar", last modified: Fri Aug  4 08:15:28 2023, max compression
+gzip compressed data, was "cybrex-1.2.6.tar", last modified: Fri Aug  4 09:11:32 2023, max compression
```

## Comparing `cybrex-1.2.4.tar` & `cybrex-1.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-04 08:15:28.977414 cybrex-1.2.4/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.2.4/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-04 08:15:28.976925 cybrex-1.2.4/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.2.4/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-04 08:15:28.971260 cybrex-1.2.4/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.2.4/cybrex/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     5649 2023-08-04 07:30:23.000000 cybrex-1.2.4/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)    13562 2023-08-04 08:15:13.000000 cybrex-1.2.4/cybrex/cybrex_ai.py
--rw-r--r--   0 pasha      (501) staff       (20)    13715 2023-08-04 08:04:56.000000 cybrex-1.2.4/cybrex/models.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-04 08:15:28.975798 cybrex-1.2.4/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-04 08:15:28.000000 cybrex-1.2.4/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      305 2023-08-04 08:15:28.000000 cybrex-1.2.4/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-04 08:15:28.000000 cybrex-1.2.4/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-04 08:15:28.000000 cybrex-1.2.4/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-04 08:15:28.000000 cybrex-1.2.4/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-04 08:15:28.000000 cybrex-1.2.4/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-04 08:14:17.000000 cybrex-1.2.4/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-02 11:17:07.000000 cybrex-1.2.4/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-04 08:15:28.977568 cybrex-1.2.4/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-04 09:11:32.530575 cybrex-1.2.6/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.2.6/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-04 09:11:32.529975 cybrex-1.2.6/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.2.6/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-04 09:11:32.525836 cybrex-1.2.6/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.2.6/cybrex/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5649 2023-08-04 07:30:23.000000 cybrex-1.2.6/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    13562 2023-08-04 08:15:13.000000 cybrex-1.2.6/cybrex/cybrex_ai.py
+-rw-r--r--   0 pasha      (501) staff       (20)    13933 2023-08-04 09:11:04.000000 cybrex-1.2.6/cybrex/models.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-04 09:11:32.529130 cybrex-1.2.6/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-04 09:11:32.000000 cybrex-1.2.6/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      305 2023-08-04 09:11:32.000000 cybrex-1.2.6/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-04 09:11:32.000000 cybrex-1.2.6/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-04 09:11:32.000000 cybrex-1.2.6/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-04 09:11:32.000000 cybrex-1.2.6/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-04 09:11:32.000000 cybrex-1.2.6/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-04 09:11:12.000000 cybrex-1.2.6/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-02 11:17:07.000000 cybrex-1.2.6/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-04 09:11:32.530800 cybrex-1.2.6/setup.cfg
```

### Comparing `cybrex-1.2.4/PKG-INFO` & `cybrex-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.2.4
+Version: 1.2.6
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.2.4/README.md` & `cybrex-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.2.4/cybrex/cli.py` & `cybrex-1.2.6/cybrex/cli.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.2.4/cybrex/cybrex_ai.py` & `cybrex-1.2.6/cybrex/cybrex_ai.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.2.4/cybrex/models.py` & `cybrex-1.2.6/cybrex/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,35 +16,33 @@
         return {
             'default': BasePrompter(),
             'llama2-7b': Llama27bPrompter(),
             'openai': OpenAIPrompter()
         }[type_]
 
     def qa_prompt(self, question, documents: List[dict]):
-        if len(documents) > 1:
+        if len(documents) >= 1:
             return '''
 USER: You are Cybrex AI created by People of Nexus. Given the following extracted parts of a long document and a question, create a final answer.
 ALWAYS add references to extracted parts using template "DOI: 10.1038/s41576-022-00477-6" near corresponding statements. 
 If you don't know the answer, just say that you don't know. Don't try to make up an answer.
 Extracted parts:
 {summary}
 
 Question:
 {question}
 ASSISTANT:'''.format(question=question, summary=self.generate_summary(documents))
         else:
             return '''
-USER: You are Cybrex AI created by People of Nexus. Given the following extracted parts of a long document and a question, create a final answer.
+USER: You are Cybrex AI created by People of Nexus. Answer the question.
 If you don't know the answer, just say that you don't know. Don't try to make up an answer.
-Extracted parts:
-{summary}
 
 Question:
 {question}
-ASSISTANT:'''.format(question=question, summary=self.generate_summary(documents))
+ASSISTANT:'''.format(question=question)
 
     def generate_summary(self, documents: List[dict]):
         document_summaries = []
         document_summaries_grouped = OrderedDict()
         for document in documents:
             if document["metadata"]["doi"] not in document_summaries_grouped:
                 document_summaries_grouped[document["metadata"]["doi"]] = []
@@ -53,27 +51,38 @@
             texts = ' <..> '.join(texts)
             document_summaries.append(f'DOI: {doi}\nCONTENT: {texts}')
         return '\n'.join(document_summaries)
 
 
 class Llama27bPrompter(BasePrompter):
     def qa_prompt(self, question: str, documents: List[dict]):
-        return '''
+        if len(documents) >= 1:
+            return '''
 <s><<SYS>>
 You are Cybrex AI created by People of Nexus. Given the following extracted parts of a long document and a question, create a final answer.
 ALWAYS add references to extracted parts using template "DOI: 10.1038/s41576-022-00477-6" near corresponding statements. 
 If you don't know the answer, just say that you don't know. Don't try to make up an answer.
 <</SYS>>
 [INST]
 Extracted parts:
 {summary}
 
 Question:
 {question}
 [/INST]'''.format(question=question, summary=self.generate_summary(documents))
+        else:
+            return '''
+<s><<SYS>>
+You are Cybrex AI created by People of Nexus. Answer the question.
+If you don't know the answer, just say that you don't know. Don't try to make up an answer.
+<</SYS>>
+[INST]
+Question:
+{question}
+[/INST]'''.format(question=question, summary=self.generate_summary(documents))
 
 
 class OpenAIPrompter(BasePrompter):
     def qa_prompt(self, question: str, documents: List[dict]):
         return """Given the following extracted parts of a long document and a question, create a final answer with references ("DOIs"). 
 If you don't know the answer, just say that you don't know. Don't try to make up an answer.
 ALWAYS return a "DOIs" part in your answer.
```

### Comparing `cybrex-1.2.4/cybrex.egg-info/PKG-INFO` & `cybrex-1.2.6/cybrex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.2.4
+Version: 1.2.6
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.2.4/pyproject.toml` & `cybrex-1.2.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.2.4"
+version = "1.2.6"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

