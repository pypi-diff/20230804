# Comparing `tmp/promptz-0.0.8.tar.gz` & `tmp/promptz-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptz-0.0.8.tar", last modified: Thu Jul 27 14:01:55 2023, max compression
+gzip compressed data, was "promptz-0.0.9.tar", last modified: Wed Aug  2 11:10:20 2023, max compression
```

## Comparing `promptz-0.0.8.tar` & `promptz-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-27 14:01:55.297938 promptz-0.0.8/
--rw-r--r--   0 rjl       (1000) rjl       (1000)    11357 2023-07-26 07:18:43.000000 promptz-0.0.8/LICENSE
--rw-r--r--   0 rjl       (1000) rjl       (1000)      187 2023-07-27 14:01:55.297938 promptz-0.0.8/PKG-INFO
--rw-r--r--   0 rjl       (1000) rjl       (1000)    14911 2023-07-26 07:07:09.000000 promptz-0.0.8/README.md
-drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-27 14:01:55.297938 promptz-0.0.8/promptz/
--rw-r--r--   0 rjl       (1000) rjl       (1000)    38207 2023-07-27 10:06:43.000000 promptz-0.0.8/promptz/__init__.py
-drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-27 14:01:55.297938 promptz-0.0.8/promptz.egg-info/
--rw-r--r--   0 rjl       (1000) rjl       (1000)      187 2023-07-27 14:01:55.000000 promptz-0.0.8/promptz.egg-info/PKG-INFO
--rw-r--r--   0 rjl       (1000) rjl       (1000)      200 2023-07-27 14:01:55.000000 promptz-0.0.8/promptz.egg-info/SOURCES.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)        1 2023-07-27 14:01:55.000000 promptz-0.0.8/promptz.egg-info/dependency_links.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)     2089 2023-07-27 14:01:55.000000 promptz-0.0.8/promptz.egg-info/requires.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)        8 2023-07-27 14:01:55.000000 promptz-0.0.8/promptz.egg-info/top_level.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)       38 2023-07-27 14:01:55.297938 promptz-0.0.8/setup.cfg
--rw-r--r--   0 rjl       (1000) rjl       (1000)      278 2023-07-27 14:01:45.000000 promptz-0.0.8/setup.py
+drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-08-02 11:10:20.924920 promptz-0.0.9/
+-rw-r--r--   0 rjl       (1000) rjl       (1000)    11357 2023-07-26 07:18:43.000000 promptz-0.0.9/LICENSE
+-rw-r--r--   0 rjl       (1000) rjl       (1000)       27 2023-08-02 11:09:02.000000 promptz-0.0.9/MANIFEST.in
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      187 2023-08-02 11:10:20.924920 promptz-0.0.9/PKG-INFO
+-rw-r--r--   0 rjl       (1000) rjl       (1000)    14911 2023-07-26 07:07:09.000000 promptz-0.0.9/README.md
+drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-08-02 11:10:20.924920 promptz-0.0.9/promptz/
+-rw-r--r--   0 rjl       (1000) rjl       (1000)    50593 2023-08-02 11:09:02.000000 promptz-0.0.9/promptz/__init__.py
+-rw-r--r--   0 rjl       (1000) rjl       (1000)     4225 2023-08-02 11:09:02.000000 promptz-0.0.9/promptz/cli.py
+drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-08-02 11:10:20.924920 promptz-0.0.9/promptz.egg-info/
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      187 2023-08-02 11:10:20.000000 promptz-0.0.9/promptz.egg-info/PKG-INFO
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      261 2023-08-02 11:10:20.000000 promptz-0.0.9/promptz.egg-info/SOURCES.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)        1 2023-08-02 11:10:20.000000 promptz-0.0.9/promptz.egg-info/dependency_links.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)       41 2023-08-02 11:10:20.000000 promptz-0.0.9/promptz.egg-info/entry_points.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)     2089 2023-08-02 11:10:20.000000 promptz-0.0.9/promptz.egg-info/requires.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)        8 2023-08-02 11:10:20.000000 promptz-0.0.9/promptz.egg-info/top_level.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)       38 2023-08-02 11:10:20.924920 promptz-0.0.9/setup.cfg
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      381 2023-08-02 11:10:00.000000 promptz-0.0.9/setup.py
```

### Comparing `promptz-0.0.8/LICENSE` & `promptz-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `promptz-0.0.8/README.md` & `promptz-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `promptz-0.0.8/promptz/__init__.py` & `promptz-0.0.9/promptz/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,51 @@
 import os
+import glob
+import importlib
+import threading
 import inspect
 import logging
 import random
 import uuid
 import textwrap
+import base64
 import json
 from json import JSONDecodeError
 from enum import Enum
-from typing import Type, Callable, List, Tuple, Dict, Union, Any, Literal 
+from typing import Type, Callable, List, Tuple, Dict, Union, Any, get_origin, get_args
 from abc import abstractmethod
-import base64
 from IPython.display import display, HTML, Image
+import requests
 import torch
 from torch import nn
 import numpy as np
 import pandas as pd
 from jinja2 import Template
+import nbformat
+from nbconvert import HTMLExporter
+from dash import Dash, html, dcc, dash_table, page_container, page_registry, register_page, callback_context
+from dash.exceptions import PreventUpdate
+from dash.dependencies import Output, Input, State
+from dash_dangerously_set_inner_html import DangerouslySetInnerHTML
+import dash_bootstrap_components as dbc
 from pydantic import BaseModel, ValidationError 
 from datetime import datetime
 from transformers import PreTrainedModel, PreTrainedTokenizer, LlamaForCausalLM, LlamaTokenizer
+from fastapi import FastAPI, HTTPException
+from fastapi.middleware.wsgi import WSGIMiddleware
 import openai
 from openai.error import RateLimitError
 import chromadb
 import colorama
 
 colorama.just_fix_windows_console()
 
+API_URL = os.getenv('API_URL', 'http://localhost:8000')
+
+
 FORMAT_INSTRUCTIONS = logging.DEBUG + 1
 CONTEXT = logging.DEBUG + 2
 EXAMPLES = logging.DEBUG + 3
 METRICS = logging.DEBUG + 4
 HISTORY = logging.DEBUG + 5
 INSTRUCTIONS = logging.INFO + 1
 INPUT = logging.INFO + 2
@@ -159,14 +175,15 @@
                 input_tokens=len(x),
                 output_tokens=len(text),
             )
         )
 
 
 class ChatLog(BaseModel):
+    prompt: str = None
     input: str = None
     output: str = None
 
 
 class ChatGPT(LLM):
     model = 'gpt-3.5-turbo'
     context = '''
@@ -364,62 +381,79 @@
 class Prompt(nn.Module):
     '''
     Follow the pattern shown in the examples below and
     generate a new output using the same format.
     '''
 
     template = """
+    INSTRUCTIONS
+    ---
     {{instructions}}
     {{format}}
     {{examples}}
     {{input}}
     {{output}}
     """
 
     input_template = """
-    INPUT: {{input}}
+    INPUT
+    ---
+    {{input}}
+    END_INPUT
     """
 
     output_template = """
-    OUTPUT: {{output}}
+    OUTPUT
+    ---
+    {{output}}
     """
 
     example_template = f"""
+    EXAMPLES
+    ---
     {input_template}
     {output_template}
+    END_EXAMPLES
     """
 
     format_template = """
+    FORMAT INSTRUCTIONS
+    ---
     {% if list_output %}
     Return a list of valid JSON objects with the fields described below.
     {% else %}
     Return the output as a valid JSON object with the fields described below. 
     {% endif %}
     {% for field in fields %}
     - {{field.name}} (type: {{field.type_}}, required: {{field.required}}){% if field.instructions != None %}: {{field.instructions}}{% endif %}
     {% endfor %}
 
     Make sure to use double quotes and avoid trailing commas!
     Ensure any required fields are set, but you can use the default value 
     if it's defined and you are unsure what to use. 
     If you are unsure about any optional fields use `null` or the default value,
     but try your best to fill them out.
+    END_FORMAT_INSTRUCTIONS
     """
 
+    id: str 
+    name: str = None
     instructions: str = None
     context: str = None
     history: List[ChatLog] = []
     examples: List[Tuple[(str|BaseModel), (str|BaseModel)]] = []
     num_examples: int = 1
     output: Type[BaseModel] = None
     llm: LLM = MockLLM()
 
-    def __init__(self, instructions=None, output=None, context=None, template=None, examples=None, num_examples=None, history=None, llm=None, logger=None, debug=False, silent=False, tools: ToolList = None):
+    def __init__(self, instructions=None, output=None, context=None, template=None, examples=None, num_examples=None, history=None, llm=None, logger=None, debug=False, silent=False, tools: ToolList = None, name=None):
         super().__init__()
 
+        self.id = str(uuid.uuid4())
+        self.name = name
         self.logger = logger
         self.name = self.__class__.__name__
         self.llm = llm or self.llm
         self.context = context or self.context
         self.history = history or self.history
         self.output = output or self.output
         instructions = instructions or self.__doc__
@@ -473,26 +507,33 @@
         }
         output = self.template.render(**vars)
         return output
     
     def format_field(self, field):
         instructions = field.field_info.description or ''
         options = ''
-        type_ = field.outer_type_
+        outer_type_ = field.outer_type_.__name__
         if issubclass(field.type_, BaseModel):
             return None
-        if field.type_ is Literal or type_ is Literal:
-            options += f'Select only one option: {", ".join(field.type_.__args__)}'
-        elif isinstance(field.type_, List):
-            item_type = field.type_.__args__[0]
+
+        if get_origin(field.outer_type_) is list:
+            item_type = get_args(field.outer_type_)[0]
             type_ = f'{item_type.__name__}[]'
-        elif isinstance(type_, type(Enum)):
+            if isinstance(item_type, type(Enum)):
+                type_ = 'str[]'
+                options += f'''Select any relevant options from: {", ".join([
+                    member.value for member in item_type
+                ])}'''
+        elif isinstance(field.type_, type(Enum)):
+            type_ = 'str'
             options += f'''Select only one option: {", ".join([
                 member.value for member in field.type_
             ])}'''
+        else:
+            type_ = field.type_.__name__
 
         if len(options) > 0:
             instructions += ' ' + options
 
         return {
             'name': field.name,
             'type_': type_,
@@ -508,15 +549,15 @@
         list_output = False
         cls = self.output
         if getattr(self.output, '__origin__', None) is list:
             # if so, get the type of the list
             list_output = True
             item_type = self.output.__args__[0]
             if item_type is str:
-                return 'Return a list of strings with double quotes around each string.'
+                return 'Return an array of strings wrapped in double quotes.'
             else:
                 cls = item_type
         fields = [self.format_field(f) for f in cls.__fields__.values()]
         return self.format_template.render({
             'fields': [field for field in fields if field is not None], 
             'list_output': list_output,
         })
@@ -551,14 +592,21 @@
                 d = json.loads(output)
                 d = {'type': type_, **d}
                 return self.output(**d)
             return Collection(rows)
         else:
             return output
     
+    def dict(self):
+        return {
+            'id': self.id,
+            'name': self.name,
+            'instructions': self.instructions,
+        }
+    
     def forward(self, x, retries=3, dryrun=False, **kwargs):
         if retries and retries <= 0:
             e = MaxRetriesExceeded(f'{self.name} failed to forward {x}')
             self.logger.error(e)
             raise e
         
         if dryrun:
@@ -576,14 +624,15 @@
             {log.input}
             {log.output}
             ''' for log in self.history]))
             self.logger.log(INSTRUCTIONS, self.instructions)
             if len(self.examples): self.logger.log(EXAMPLES, self.render_examples())
             if len(px): self.logger.log(INPUT, px)
             tools = [t.info for t in self.tools]
+            self.logger.debug(f'FULL INPUT: {prompt_input}')
             response = llm.generate(prompt_input, context=self.context, history=self.history, tools=tools)
             if response.callback is not None:
                 function_name = response.callback.name
                 tool = next(t for t in self.tools if t.name == function_name)
                 params = {p['name']: response.callback.params.get(p['name']) 
                           for p in tool.parameters}
                 rsp = tool(**params)
@@ -601,20 +650,18 @@
             except RateLimitError as e:
                 self.logger.warn(f'Hit rate limit for {self}: {e}')
                 return self.forward(x, retries=retries-1, **kwargs)
             self.logger.log(METRICS, response.metrics)
             return response
 
 
-class Query:
-
-    def __init__(self, query=None, where=None, collection=None, **kwargs):
-        self.query = query
-        self.where = where or {}
-        self.collection = collection
+class Query(BaseModel):
+    query: str
+    where: Dict[str, Any] = None
+    collection: str = None
 
 
 class ChatPrompt(Prompt):
     '''
     You are a helpful assistant.
     '''
 
@@ -875,27 +922,30 @@
                         return Response(
                             raw=r.output,
                             cached=True,
                             content=p.process(input, r.output, **kwargs),
                         )
 
             r = p(input, dryrun=dryrun, retries=retries, **kwargs)
-            log = ChatLog(input=rendered, output=r.raw)
+            log = ChatLog(prompt=p.id, input=rendered, output=r.raw)
             self._history.append(log)
             collection = self.collection('history')
             collection.embed(log)
             return r
         except MaxRetriesExceeded as e:
             self.logger.error(f'Max retries exceeded: {e}')
             return None
     
     def _run_batch(self, p, inputs, dryrun=False, retries=3, **kwargs):
+        o = []
         for input in inputs:
-            o = self._run_prompt(p, input, dryrun=dryrun, retries=retries, **kwargs)
-            yield o.content
+            r = self._run_prompt(p, input, dryrun=dryrun, retries=retries, **kwargs)
+            if r is not None:
+                o.append(r.content)
+        return o
 
     def prompt(self, instructions=None, input=None, output=None, prompt=None, context=None, template=None, llm=None, examples=None, num_examples=1, history=None, tools=None, dryrun=False, retries=3, debug=False, silent=False, **kwargs):
         logger = self.logger.getChild('prompt')
         level = logging.INFO
         if debug: level = logging.DEBUG
         elif silent: level = logging.ERROR
         logger.setLevel(level)
@@ -922,14 +972,16 @@
             p.debug = debug
             p.silent = silent
 
         if isinstance(input, list):
             o = self._run_batch(p, input, dryrun=dryrun, retries=retries, **kwargs)
         else:
             r = self._run_prompt(p, input, dryrun=dryrun, retries=retries, **kwargs)
+            if r is None:
+                return None
             o = r.content
         return o
     
     def embed(self, item, field=None):
         if isinstance(item, str):
             return self.ef([item])[0]
         elif isinstance(item, BaseModel):
@@ -1054,52 +1106,357 @@
         return self.process(*args, **kwds)
 
 
 class World:
     name: str
     sessions: List[Session]
     collections: Dict[str, Collection]
-    systems: List[System]
+    systems: Dict[str, System]
+    prompts: Dict[str, Prompt]
+    notebooks: Dict[str, str]
 
-    def __init__(self, name, systems=None, llm=None, ef=None, logger=None, db=None):
+    def __init__(self, name, systems=None, llm=None, ef=None, logger=None, db=None, prompts=None, notebooks=None):
         self.name = name
         self.sessions = []
         self.collections = {}
-        self.systems = systems
         self.llm = llm or MockLLM()
         self.ef = ef or (lambda x: [0] * len(x))
-        self.db = db or ChromaVectorDB
+        self.db = db or ChromaVectorDB()
         self.logger = logger or logging.getLogger(self.name)
+        self.prompts = prompts or {}
+        self.systems = systems or {}
+        self.notebooks = notebooks or {}
+
+        collection = self.db.get_or_create_collection('history', metadata={"hnsw:space": "cosine"})
+        self.collections['history'] = collection
     
     def create_session(self, name=None, db=None, llm=None, ef=None, logger=None, silent=False, debug=False, use_cache=False, log_format='notebook'):
         llm = llm or self.llm
         ef = ef or self.ef
-        db = db or self.db()
+        db = db or self.db
         logger = logger or self.logger.getChild(f'session.{name}')
         ch = logging.StreamHandler()
         formatter = JSONLogFormatter() if log_format == 'json' else NotebookFormatter()
         ch.setFormatter(formatter)
         self.logger.addHandler(ch)
         level = logging.INFO
         if debug: level = logging.DEBUG
         elif silent: level = logging.ERROR
         logger.setLevel(level)
         session = Session(name=name, db=db, llm=llm, ef=ef, logger=logger,
                           collections=self.collections, use_cache=use_cache)
-        self.sessions = self.sessions.append(session)
+        self.sessions.append(session)
         return session
     
-    def __call__(self, *args: Any, **kwds: Any) -> Any:
-        session = self.create_session(
-            f'{self.__class__.__name__}.session-{uuid.uuid4()}')
-        for system in self.systems:
+    def __call__(self, session, *args: Any, **kwds: Any) -> Any:
+        for system in self.systems.values():
             items = session.query(system.query)
             updates = system(items)
             session.store(updates)
-        return session
+
+
+class PromptInput(BaseModel):
+    input: Any
+
+
+class API:
+    world: World
+
+    def __init__(self, world):
+        self.world = world
+        self.fastapi_app = FastAPI()
+        
+        @self.fastapi_app.get("/prompts")
+        async def get_prompts():
+            return {"response": {k: v.dict() for k, v in self.world.prompts.items()}}
+
+        @self.fastapi_app.get("/prompts/{id}")
+        async def get_prompt(id: str):
+            history = self.world.collections['history']
+            c = Collection.load(history)
+            if c.empty:
+                results = []
+            else:
+                results = c[c['prompt'] == id].to_dict('records')
+            prompt = self.world.prompts[id]
+            print('results', results, c, id)
+            return {'prompt': prompt, 'results': results}
+
+        @self.fastapi_app.post("/prompts/{name}/run")
+        async def run_prompt(name: str, input: PromptInput = None):
+            session = self.world.create_session()
+            if name not in self.world.prompts:
+                raise HTTPException(status_code=404, detail="Prompt not found")
+            prompt_config = self.world.prompts[name]
+            d = {**prompt_config, 'input': input}
+            response = session.prompt(**{**prompt_config, 'input': input})
+            return {"response": response}
+        
+        @self.fastapi_app.get("/systems")
+        async def get_systems():
+            return {"response": self.world.systems.keys()}
+        
+        @self.fastapi_app.get("/systems/{name}")
+        async def get_system(name: str):
+            return {"response": self.world.systems[name]}
+        
+        @self.fastapi_app.post("/systems/run")
+        async def run_systems():
+            session = self.world.create_session()
+            return {"response": self.world(session)}
+        
+        @self.fastapi_app.post("/query")
+        async def query(query: Query):
+            session = self.world.create_session()
+            response = session.query(query.query, where=query.where, collection=query.collection)
+            return {"response": response}
+        
+        @self.fastapi_app.get("/notebooks")
+        async def get_notebooks():
+            return {"response": self.world.notebooks}
+        
+        @self.fastapi_app.get("/notebooks/{name}")
+        async def get_notebook(name: str):
+            return {"response": self.world.notebooks[name]}
+        
+        @self.fastapi_app.get("/chats")
+        async def get_chats():
+            return {"response": {}}
+
+
+class Admin:
+    world: World
+
+    def __init__(self, world):
+        self.world = world
+        self.app = Dash(
+            world.name, 
+            use_pages=True,
+            pages_folder='admin',
+            external_stylesheets=[dbc.themes.ZEPHYR],
+        )
+
+        register_page(
+            'Inbox',
+            layout=html.Div(children=[
+            ]),
+            path='/',
+        )
+
+        def prompts_list_layout():
+            response = requests.get(f'{API_URL}/prompts')
+            if response.status_code == 200:
+                prompts = response.json()
+            else:
+                raise Exception(f'Error getting prompts: {response.status_code}')
+            
+            print('prompts', prompts)
+            return html.Div(children=[
+                html.H1(children='Prompts'),
+                html.Ul([
+                    html.Li(html.A(p['name'], href=f'/prompts/{id}')) for id, p in prompts['response'].items()
+                ]),
+            ])
+
+        register_page(
+            'Prompts',
+            layout=prompts_list_layout,
+            path='/prompts',
+        )
+
+        def prompt_layout(id: str = None):
+            response = requests.get(f'{API_URL}/prompts/{id}')
+            if response.status_code == 200:
+                data = response.json()
+                prompt = data['prompt']
+                results = data['results']
+            else:
+                raise Exception(f'Error getting prompt: {response.status_code}')
+
+            return html.Div(children=[
+                html.H1(id),
+                dbc.Button('Run', id='run-prompt', n_clicks=0, name=id, color='primary'),
+                dcc.Store(id='api-call-result', storage_type='session'),
+                html.Div(id, id='prompt-id', style={'display': 'none'}),
+                html.Div(id='prompt-results', children=[
+                    html.P(result) for result in results
+                ]),
+            ])
+
+        register_page('Prompt', layout=prompt_layout, path_template='/prompts/<id>')
+
+        @self.app.callback(
+            Output('api-call-result', 'data'),
+            [Input('run-prompt', 'n_clicks')],
+            [State('api-call-result', 'data'),
+             State('prompt-id', 'children')],
+        )
+        def run_prompt(n_clicks, current_data, id):
+            if n_clicks is None or n_clicks == 0:
+                raise PreventUpdate
+            else:
+                requests.post(f'{API_URL}/prompts/{id}/run')
+
+        def systems_list_layout():
+            response = requests.get(f'{API_URL}/systems')
+            if response.status_code == 200:
+                systems = response.json()
+            else:
+                raise Exception(f'Error getting systems: {response.status_code}')
+            
+            return html.Div(children=[
+                html.H1(children='Systems'),
+                html.Ul([
+                    html.Li(html.A(name, href=f'/systems/{name}')) for name in systems['response'].keys()
+                ]),
+            ])
+
+        register_page(
+            'Systems',
+            layout=systems_list_layout,
+            path='/systems',
+        )
+
+        def notebook_list_layout():
+            response = requests.get(f'{API_URL}/notebooks')
+            if response.status_code == 200:
+                notebooks = response.json()
+            else:
+                raise Exception(f'Error getting notebooks: {response.status_code}')
+            
+            return html.Div(children=[
+                html.H1(children='Notebooks'),
+                html.Ul([
+                    html.Li(html.A(name, href=f'/notebooks/{name}')) for name in notebooks['response'].keys()
+                ]),
+            ])
+
+        register_page(
+            'Notebooks',
+            layout=notebook_list_layout,
+            path='/notebooks',
+        )
+
+        def notebook_layout(name: str = None):
+            response = requests.get(f'{API_URL}/notebooks/{name}')
+            notebook_html = response.json()['response']
+            return html.Div(children=[
+                html.H1(name),
+                DangerouslySetInnerHTML(notebook_html)
+            ])
+
+        register_page('Notebook', layout=notebook_layout, path_template='/notebooks/<name>')
+
+        def chatbots_list_layout():
+            response = requests.get(f'{API_URL}/chats')
+            if response.status_code == 200:
+                chats = response.json()
+            else:
+                raise Exception(f'Error getting chats: {response.status_code}')
+            
+            return html.Div(children=[
+                html.H1(children='Chats'),
+                html.Ul([
+                    html.Li(html.A(name, href=f'/chats/{name}')) for name in chats['response'].keys()
+                ]),
+            ])
+
+        register_page(
+            'Chats',
+            layout=chatbots_list_layout,
+            path='/chats',
+        )
+
+        menu = [
+            'Prompts',
+            'Notebooks',
+        ]
+
+        self.app.layout = dbc.Row([
+            dbc.Col([
+                dbc.Row(
+                    html.H3('promptz', style={'color': 'white'})
+                ),
+                *[
+                    dbc.Row(
+                        html.Div(
+                            dcc.Link(
+                                f"{page_registry[name]['name']}", href=page_registry[name]["relative_path"],
+                                style={'color': 'white', 'text-decoration': 'none'}
+                            )
+                        ),
+                    )
+                    for name in menu
+                ]
+            ], width=3, style={'background-color': '#663399', 'padding': '10px 20px', 'height': '100vh'}),
+            dbc.Col([
+                page_container
+            ], width=9, style={'padding': '10px'}),
+        ])
+
+
+class App:
+    name: str
+    world: World
+    prompts_dir: str = 'prompts'
+    systems_dir: str = 'systems'
+    notebooks_dirs: str = ['notebooks']
+
+    def __init__(self, name, world=None, llm=None, ef=None, logger=None, db=None):
+        self.name = name
+        self.logger = logger or logging.getLogger(self.name)
+        prompts = self._load_prompts()
+        systems = self._load_systems()
+        notebooks = self._load_notebooks()
+        self.world = world or World(name, prompts=prompts, systems=systems, notebooks=notebooks, llm=llm, ef=ef, logger=logger, db=db)
+        self.api = API(self.world)
+        self.admin = Admin(self.world)
+    
+    def _load_prompts(self):
+        prompts = {}
+        for file in glob.glob(os.path.join(self.prompts_dir, '*.json')):
+            with open(file, 'r') as f:
+                prompt = Prompt(**json.load(f))
+                prompts[prompt.id] = prompt
+        self.logger.info(f'Loaded {len(prompts)} prompts: {prompts}')
+        return prompts
+    
+    def _load_notebooks(self):
+        html_notebooks = {}
+        for dir in self.notebooks_dirs:
+            for file in glob.glob(os.path.join(dir, '*.ipynb')):
+                with open(file, 'r') as f:
+                    file_name = os.path.splitext(os.path.basename(file))[0]
+                    html_exporter = HTMLExporter()
+                    notebook_node = nbformat.read(f, as_version=4)
+                    body, resources = html_exporter.from_notebook_node(notebook_node)
+                    html_notebooks[file_name] = body
+        return html_notebooks
+    
+    def _load_systems(self):
+        systems = {}
+        #for file in glob.glob(os.path.join(self.systems_dir, '*.py')):
+        #    file_name = os.path.splitext(os.path.basename(file))[0]
+        #    module = importlib.import_module(f'{self.systems_dir}.{file_name}')
+        #    systems[file_name] = module
+        return systems
+    
+    def _serve_api(self, host='0.0.0.0', port=8000):
+        import uvicorn
+        uvicorn.run(self.api.fastapi_app, host=host, port=port)
+    
+    def _serve_admin(self, host='0.0.0.0', port=8001):
+        from waitress import serve
+        serve(self.admin.app.server, host=host, port=port)
+    
+    def serve(self, host='0.0.0.0', port=8000, admin_port=8001):
+        api = threading.Thread(target=lambda: self._serve_api(host=host, port=port))
+        admin = threading.Thread(target=lambda: self._serve_admin(host=host, port=admin_port))
+        api.start()
+        admin.start()
 
 
 def prompt(instructions=None, input=None, output=None, prompt=None, context=None, template=None, llm=None, examples=None, num_examples=1, history=None, tools=None, dryrun=False, retries=3, debug=False, silent=False, **kwargs):
     kwargs = dict(
         instructions=instructions,
         input=input,
         output=output,
@@ -1174,8 +1531,8 @@
 EmbedFunction = Callable[[List[str]], List[Embedding]]
 
 
 def init(llm=None, ef=None, logger=None, use_cache=False, log_format='notebook', **kwargs):
     w = World('test', llm=llm, ef=ef, logger=logger, **kwargs)
     session = w.create_session(use_cache=use_cache, log_format=log_format)
     set_default_world(w)
-    set_default_session(session)
+    set_default_session(session)
```

### Comparing `promptz-0.0.8/promptz.egg-info/requires.txt` & `promptz-0.0.9/promptz.egg-info/requires.txt`

 * *Files identical despite different names*

