# Comparing `tmp/mereja-0.0.2.tar.gz` & `tmp/mereja-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mereja-0.0.2.tar", last modified: Fri Aug  4 15:50:30 2023, max compression
+gzip compressed data, was "mereja-0.0.3.tar", last modified: Fri Aug  4 16:44:30 2023, max compression
```

## Comparing `mereja-0.0.2.tar` & `mereja-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:50:30.423201 mereja-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-08-04 15:50:30.423201 mereja-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-08-04 15:50:20.000000 mereja-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:50:30.419201 mereja-0.0.2/mereja/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:50:30.423201 mereja-0.0.2/mereja/functions/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/functions/forex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/functions/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/functions/market.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/functions/news.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/functions/telebirr.py
--rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:50:30.423201 mereja-0.0.2/mereja/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/ui/forex_table_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/ui/job_view_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/ui/marketpalce_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/ui/news_view_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/ui/transaction_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:50:30.423201 mereja-0.0.2/mereja/ui/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/ui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/ui/widgets/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:50:30.423201 mereja-0.0.2/mereja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-08-04 15:50:30.000000 mereja-0.0.2/mereja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-04 15:50:30.000000 mereja-0.0.2/mereja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:50:30.000000 mereja-0.0.2/mereja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 15:50:30.000000 mereja-0.0.2/mereja.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-04 15:50:30.000000 mereja-0.0.2/mereja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 15:50:30.000000 mereja-0.0.2/mereja.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-04 15:50:30.423201 mereja-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-04 15:50:20.000000 mereja-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:44:30.915294 mereja-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-08-04 16:44:30.915294 mereja-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-08-04 16:44:21.000000 mereja-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:44:30.911294 mereja-0.0.3/mereja/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:44:30.915294 mereja-0.0.3/mereja/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/functions/forex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/functions/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/functions/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/functions/news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/functions/telebirr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:44:30.915294 mereja-0.0.3/mereja/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/ui/forex_table_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/ui/job_view_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/ui/marketpalce_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/ui/news_view_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/ui/transaction_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:44:30.915294 mereja-0.0.3/mereja/ui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/ui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/ui/widgets/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:44:30.911294 mereja-0.0.3/mereja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-08-04 16:44:30.000000 mereja-0.0.3/mereja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-04 16:44:30.000000 mereja-0.0.3/mereja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 16:44:30.000000 mereja-0.0.3/mereja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 16:44:30.000000 mereja-0.0.3/mereja.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-04 16:44:30.000000 mereja-0.0.3/mereja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 16:44:30.000000 mereja-0.0.3/mereja.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-04 16:44:30.915294 mereja-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-04 16:44:21.000000 mereja-0.0.3/setup.py
```

### Comparing `mereja-0.0.2/PKG-INFO` & `mereja-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mereja
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/wizkiye/mereja
 Author: Kidus
 Author-email: wizkiye@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -76,14 +76,26 @@
                         Search for a job/product/news
   --export, -e          Export to file
   --path PATH, -pa PATH
                         Path to export file
 ```
 
 ## Examples
+
+<details>
+<summary>Without any options</summary>
+
+```bash
+# Without any options
+mereja
+```
+![Made with VHS](https://vhs.charm.sh/vhs-3U79nZQbOZOCFYqxnIu0d0.gif)
+
+</details>
+
 <details>
 <summary>Get latest jobs</summary>
 
 ```bash
 # Get latest jobs
 mereja --job --latest
 ```
```

### Comparing `mereja-0.0.2/README.md` & `mereja-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,26 @@
                         Search for a job/product/news
   --export, -e          Export to file
   --path PATH, -pa PATH
                         Path to export file
 ```
 
 ## Examples
+
+<details>
+<summary>Without any options</summary>
+
+```bash
+# Without any options
+mereja
+```
+![Made with VHS](https://vhs.charm.sh/vhs-3U79nZQbOZOCFYqxnIu0d0.gif)
+
+</details>
+
 <details>
 <summary>Get latest jobs</summary>
 
 ```bash
 # Get latest jobs
 mereja --job --latest
 ```
```

### Comparing `mereja-0.0.2/mereja/constants.py` & `mereja-0.0.3/mereja/constants.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.2/mereja/functions/forex.py` & `mereja-0.0.3/mereja/functions/forex.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.2/mereja/functions/jobs.py` & `mereja-0.0.3/mereja/functions/jobs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import json
 
 from pyethiojobs import EthioJobs
 from questionary import Choice
 from rich.status import Status
 
 from mereja.ui import JobView
-from mereja.utils import ask, with_live, save_file, get_path
+from mereja.utils import ask, with_live, save_file, get_path, no_ans_or_back
 
 
 @with_live("Searching for {query}...")
 async def search_for_job(query: str, status: Status) -> None:
     jobs = await EthioJobs().search(query)
     if not jobs:
         status.console.print("[bold yellow]No jobs found")
         return
     status.console.print(f"[bold green]Found {len(jobs)} jobs")
     status.stop()
     ans = await ask(
         message="Select a job",
         choice=[Choice(job.title, value=job.job_id) for job in jobs],
     )
-    if not ans:
-        return
+    no_ans_or_back(ans)
     job = await EthioJobs().get_job(ans)
     await JobView(job).run_async()
 
 
 @with_live("Searching for government jobs...")
 async def get_government_jobs(status: Status):
     jobs = await EthioJobs().get_gov_jobs()
@@ -34,16 +33,15 @@
         return
     status.console.print(f"[bold green]Found {len(jobs)} jobs")
     status.stop()
     ans = await ask(
         message="Select a job",
         choice=[Choice(job.company, value=job.job) for job in jobs],
     )
-    if not ans:
-        return
+    no_ans_or_back(ans)
     job = await EthioJobs().get_job(ans)
     await JobView(job).run_async()
 
 
 @with_live("Searching for latest jobs...")
 async def get_latest_jobs(status: Status):
     jobs = await EthioJobs().get_latest_jobs()
@@ -52,16 +50,15 @@
         return
     status.console.print(f"[bold green]Found {len(jobs)} jobs")
     status.stop()
     ans = await ask(
         message="Select a job",
         choice=[Choice(job.title, value=job.job_id) for job in jobs],
     )
-    if not ans:
-        return
+    no_ans_or_back(ans)
     job = await EthioJobs().get_job(ans)
     await JobView(job).run_async()
 
 
 @with_live("Searching for latest jobs...")
 async def export_latest_jobs(path: str, status: Status, limit: int):
     jobs = await EthioJobs().get_latest_jobs()
```

### Comparing `mereja-0.0.2/mereja/functions/market.py` & `mereja-0.0.3/mereja/functions/market.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 
 from jiji import JiJi
 from questionary import Choice
 from rich.status import Status
 
 from mereja.ui import start_market_ui
-from mereja.utils import ask, with_live, save_file, get_path
+from mereja.utils import ask, with_live, save_file, get_path, no_ans_or_back
 
 
 @with_live("Searching for {query}...")
 async def search_for_product(
     query: str,
     status: Status,
     page: int = 1,
@@ -32,16 +32,15 @@
                 f"{product.title} - [{product.price} ETB] "
                 f"{f' ({product.price_type})' if product.price_type else ' (Fixed)'}",
                 value=product.id,
             )
             for product in products
         ],
     )
-    if not ans:
-        return
+    no_ans_or_back(ans)
     product = await jiji.get_product(ans)
     start_market_ui(product)
 
 
 @with_live("Getting trending products...")
 async def get_trending_products(status: Status, limit: int = -1, page: int = 1) -> None:
     jiji = JiJi()
@@ -59,16 +58,15 @@
                 f"{product.title} - [{product.price} ETB]"
                 f" {f' ({product.price_type})' if product.price_type else ' (Fixed)'}",
                 value=product.id,
             )
             for product in products
         ],
     )
-    if not ans:
-        return
+    no_ans_or_back(ans)
     product = await jiji.get_product(ans)
     start_market_ui(product)
 
 
 @with_live("Getting trending products...")
 async def export_products(
     status: Status,
```

### Comparing `mereja-0.0.2/mereja/functions/news.py` & `mereja-0.0.3/mereja/functions/news.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 
 from pyEthioNews.providers import VOAAmharic
 from questionary import Choice
 from rich.status import Status
 
 from mereja.ui import NewsView
-from mereja.utils import ask, with_live, save_file, get_path
+from mereja.utils import ask, with_live, save_file, get_path, no_ans_or_back
 
 
 @with_live("Searching for {query}...")
 async def search_news(
     query: str,
     status: Status,
     page: int = 1,
@@ -28,16 +28,15 @@
             Choice(
                 f"{news.title} - [{news.date}]",
                 value=news.link,
             )
             for news in news
         ],
     )
-    if not ans:
-        return
+    no_ans_or_back(ans)
     news = await voa.get(ans)
     await NewsView(news).run_async()
 
 
 @with_live("Getting latest news...")
 async def get_news(status: Status, page: int = 1) -> None:
     voa = VOAAmharic()
@@ -53,16 +52,15 @@
             Choice(
                 f"{news.title} - [{news.date}]",
                 value=news.link,
             )
             for news in news
         ],
     )
-    if not ans:
-        return
+    no_ans_or_back(ans)
     news = await voa.get(ans)
     await NewsView(news).run_async()
 
 
 @with_live("Getting latest news...")
 async def export_news(
     status: Status,
```

### Comparing `mereja-0.0.2/mereja/functions/telebirr.py` & `mereja-0.0.3/mereja/functions/telebirr.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.2/mereja/main.py` & `mereja-0.0.3/mereja/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import asyncio
 import sys
 
 import questionary
 
 from mereja import constants
 from mereja.functions import forex, telebirr, market, news, jobs
-from mereja.utils import awaitable
+from mereja.utils import awaitable, Back
 
 questions = [
     {
         "type": "select",
         "name": "answer",
         "message": "What do you want to do?",
         "choices": [
@@ -22,47 +22,52 @@
             "🛑 Exit",
         ],
     },
     {
         "type": "select",
         "name": "forex_choice",
         "message": "What do you want to do?",
-        "choices": ["📈 Get forex", "📈 🚦 Get forex Live", "📂 Export forex data", "Back"],
+        "choices": [
+            "📈 Get forex",
+            "📈 🚦 Get forex Live",
+            "📂 Export forex data",
+            "🔙 Back",
+        ],
         "qmark": "📈",
         "when": lambda answers: answers.get("answer") == "📈 Forex",
     },
     {
         "type": "select",
         "name": "choice",
         "message": "What do you want to do with news?",
-        "choices": ["📝 Get latest news", "🔍 Search for news", "Back"],
+        "choices": ["📝 Get latest news", "🔍 Search for news", "🔙 Back"],
         "qmark": "📝",
         "when": lambda answers: answers.get("answer") == "📝 News",
     },
     {
         "type": "select",
         "name": "choice",
         "message": "What do you want to do with jobs?",
-        "choices": ["Get latest jobs", "🔍 Search for jobs", "Back"],
+        "choices": ["Get latest jobs", "🔍 Search for jobs", "🔙 Back"],
         "qmark": "💼",
         "when": lambda answers: answers.get("answer") == "💼 Jobs",
     },
     {
         "type": "select",
         "name": "choice",
         "message": "What do you want to do with marketplace?",
-        "choices": ["📈 Get trending products", "🔍 Search for products", "Back"],
+        "choices": ["📈 Get trending products", "🔍 Search for products", "🔙 Back"],
         "qmark": "🛍",
         "when": lambda answers: answers.get("answer") == "🛍 Marketplace",
     },
     {
         "type": "select",
         "name": "telebirr_choice",
         "message": "What do you want to do with telebirr?",
-        "choices": ["💳 Transaction Details", "📂 Export transaction data", "Back"],
+        "choices": ["💳 Transaction Details", "📂 Export transaction data", "🔙 Back"],
         "qmark": "💳",
         "when": lambda answers: answers.get("answer") == "💳 Telebirr",
     },
     {
         "type": "text",
         "name": "transaction_id",
         "message": "💳 Enter your transaction ID:",
@@ -126,63 +131,62 @@
 
         elif answers.get("forex_choice") == "📈 🚦 Get forex Live":
             await forex.get_forex(live=True)
 
         elif answers.get("forex_choice") == "📂 Export forex data":
             await forex.export_forex_data(path=answers.get("path"))
 
-        elif answers.get("forex_choice") == "Back":
+        elif answers.get("forex_choice") == "🔙 Back":
             return
     elif answers.get("answer") == "📝 News":
         if answers.get("choice") == "📝 Get latest news":
             await news.get_news(page=answers.get("page"))
 
         elif answers.get("choice") == "🔍 Search for news":
             await news.search_news(
                 query=answers.get("search"), page=answers.get("page")
             )
 
-        elif answers.get("choice") == "Back":
+        elif answers.get("choice") == "🔙 Back":
             return
 
     elif answers.get("answer") == "💼 Jobs":
         if answers.get("choice") == "Get latest jobs":
             await jobs.get_latest_jobs()
 
         elif answers.get("choice") == "🔍 Search for jobs":
             await jobs.search_for_job()
 
-        elif answers.get("choice") == "Back":
+        elif answers.get("choice") == "🔙 Back":
             return
-
     elif answers.get("answer") == "🛍 Marketplace":
         if answers.get("choice") == "📈 Get trending products":
             await market.get_trending_products()
 
         elif answers.get("choice") == "🔍 Search for products":
             await market.search_for_product(
                 query=answers.get("search"), page=answers.get("page")
             )
 
-        elif answers.get("choice") == "Back":
+        elif answers.get("choice") == "🔙 Back":
             return
 
     elif answers.get("answer") == "💳 Telebirr":
         if answers.get("telebirr_choice") == "💳 Transaction Details":
             await telebirr.check_transaction(
                 transaction_id=answers.get("transaction_id")
             )
 
         elif answers.get("telebirr_choice") == "📂 Export transaction data":
             await telebirr.export_transaction(
                 path=answers.get("path"),
                 transaction_id=answers.get("transaction_id"),
             )
 
-        elif answers.get("telebirr_choice") == "Back":
+        elif answers.get("telebirr_choice") == "🔙 Back":
             return
 
     elif answers.get("answer") == "🛑 Exit":
         if answers.get("exit"):
             sys.exit(0)
```

### Comparing `mereja-0.0.2/mereja/ui/forex_table_ui.py` & `mereja-0.0.3/mereja/ui/forex_table_ui.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.2/mereja/ui/job_view_ui.py` & `mereja-0.0.3/mereja/ui/job_view_ui.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.2/mereja/ui/marketpalce_ui.py` & `mereja-0.0.3/mereja/ui/marketpalce_ui.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.2/mereja/ui/news_view_ui.py` & `mereja-0.0.3/mereja/ui/news_view_ui.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.2/mereja/ui/transaction_table.py` & `mereja-0.0.3/mereja/ui/transaction_table.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.2/mereja/ui/widgets/header.py` & `mereja-0.0.3/mereja/ui/widgets/header.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.2/mereja/utils.py` & `mereja-0.0.3/mereja/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 from questionary import Choice
 from rich.console import Console
 from rich.table import Table
 
 from mereja import constants
 
 
+class Back(Exception):
+    pass
+
+
 def random_spinner():
     return random.choice(constants.SPINNERS)
 
 
 def rmv_etb(text: str) -> float:
     if isinstance(text, str):
         return round(float(re.search(r"(\d+\.\d+)", text).group(1)), 4)
@@ -68,14 +72,21 @@
 def loop_row(table: Table, rows: list[tuple]):
     for row in rows:
         with beat(5):
             table.add_row(*row)
 
 
 async def ask(message: str, choice: list[Choice]):
+    # choice.append(
+    #     Choice(
+    #         title="🔙 Back",
+    #         value="back",
+    #     )
+    # )
+
     return await questionary.select(
         message=message,
         choices=choice,
         qmark="📝",
         style=constants.STYLE,
         use_arrow_keys=True,
         use_jk_keys=True,
@@ -107,16 +118,17 @@
             ) as status:
                 try:
                     await func(*args, **kwargs, status=status)
                 except ConnectError:
                     console.print("[bold red]No internet connection.")
                     exit(1)
                 except KeyboardInterrupt:
-                    print("Exiting...")
-                    exit(0)
+                    # print("Exiting...")
+                    # exit(0)
+                    return
                 except ConnectTimeout:
                     console.print("[bold red]Connection timeout.")
                     exit(1)
                 except Exception as e:
                     print(e)
                     exit(1)
 
@@ -139,7 +151,12 @@
     async def run(*args, loop=None, executor=None, **kwargs):
         if loop is None:
             loop = asyncio.get_event_loop()
         pfunc = partial(func, *args, **kwargs)
         return await loop.run_in_executor(executor, pfunc)
 
     return run
+
+
+def no_ans_or_back(ans: str):
+    if not ans:
+        raise KeyboardInterrupt
```

### Comparing `mereja-0.0.2/mereja.egg-info/PKG-INFO` & `mereja-0.0.3/mereja.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mereja
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/wizkiye/mereja
 Author: Kidus
 Author-email: wizkiye@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -76,14 +76,26 @@
                         Search for a job/product/news
   --export, -e          Export to file
   --path PATH, -pa PATH
                         Path to export file
 ```
 
 ## Examples
+
+<details>
+<summary>Without any options</summary>
+
+```bash
+# Without any options
+mereja
+```
+![Made with VHS](https://vhs.charm.sh/vhs-3U79nZQbOZOCFYqxnIu0d0.gif)
+
+</details>
+
 <details>
 <summary>Get latest jobs</summary>
 
 ```bash
 # Get latest jobs
 mereja --job --latest
 ```
```

### Comparing `mereja-0.0.2/mereja.egg-info/SOURCES.txt` & `mereja-0.0.3/mereja.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mereja-0.0.2/setup.py` & `mereja-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_file(filename: str):
     with open(filename, encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="mereja",
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(),
     url="https://github.com/wizkiye/mereja",
     license="MIT",
     author="Kidus",
     author_email="wizkiye@gmail.com",
     description="",
     install_requires=[
```

