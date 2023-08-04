# Comparing `tmp/mereja-0.0.3.tar.gz` & `tmp/mereja-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mereja-0.0.3.tar", last modified: Fri Aug  4 16:44:30 2023, max compression
+gzip compressed data, was "mereja-0.0.4.tar", last modified: Fri Aug  4 17:16:43 2023, max compression
```

## Comparing `mereja-0.0.3.tar` & `mereja-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:44:30.915294 mereja-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-08-04 16:44:30.915294 mereja-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-08-04 16:44:21.000000 mereja-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:44:30.911294 mereja-0.0.3/mereja/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:44:30.915294 mereja-0.0.3/mereja/functions/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/functions/forex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/functions/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/functions/market.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/functions/news.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/functions/telebirr.py
--rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:44:30.915294 mereja-0.0.3/mereja/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/ui/forex_table_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/ui/job_view_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/ui/marketpalce_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/ui/news_view_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/ui/transaction_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:44:30.915294 mereja-0.0.3/mereja/ui/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/ui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/ui/widgets/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-04 16:44:21.000000 mereja-0.0.3/mereja/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:44:30.911294 mereja-0.0.3/mereja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-08-04 16:44:30.000000 mereja-0.0.3/mereja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-04 16:44:30.000000 mereja-0.0.3/mereja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 16:44:30.000000 mereja-0.0.3/mereja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 16:44:30.000000 mereja-0.0.3/mereja.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-04 16:44:30.000000 mereja-0.0.3/mereja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 16:44:30.000000 mereja-0.0.3/mereja.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-04 16:44:30.915294 mereja-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-04 16:44:21.000000 mereja-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:16:43.630593 mereja-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-08-04 17:16:43.630593 mereja-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-08-04 17:16:31.000000 mereja-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:16:43.626593 mereja-0.0.4/mereja/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-04 17:16:31.000000 mereja-0.0.4/mereja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-04 17:16:31.000000 mereja-0.0.4/mereja/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:16:43.626593 mereja-0.0.4/mereja/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 17:16:31.000000 mereja-0.0.4/mereja/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-04 17:16:31.000000 mereja-0.0.4/mereja/functions/forex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-08-04 17:16:31.000000 mereja-0.0.4/mereja/functions/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-08-04 17:16:31.000000 mereja-0.0.4/mereja/functions/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-08-04 17:16:31.000000 mereja-0.0.4/mereja/functions/news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-04 17:16:31.000000 mereja-0.0.4/mereja/functions/telebirr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-08-04 17:16:31.000000 mereja-0.0.4/mereja/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:16:43.630593 mereja-0.0.4/mereja/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-04 17:16:31.000000 mereja-0.0.4/mereja/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-08-04 17:16:31.000000 mereja-0.0.4/mereja/ui/forex_table_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-04 17:16:31.000000 mereja-0.0.4/mereja/ui/job_view_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-08-04 17:16:31.000000 mereja-0.0.4/mereja/ui/marketpalce_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-04 17:16:31.000000 mereja-0.0.4/mereja/ui/news_view_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-08-04 17:16:31.000000 mereja-0.0.4/mereja/ui/transaction_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:16:43.630593 mereja-0.0.4/mereja/ui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 17:16:31.000000 mereja-0.0.4/mereja/ui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-08-04 17:16:31.000000 mereja-0.0.4/mereja/ui/widgets/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-08-04 17:16:31.000000 mereja-0.0.4/mereja/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:16:43.626593 mereja-0.0.4/mereja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-08-04 17:16:43.000000 mereja-0.0.4/mereja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-04 17:16:43.000000 mereja-0.0.4/mereja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 17:16:43.000000 mereja-0.0.4/mereja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 17:16:43.000000 mereja-0.0.4/mereja.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-04 17:16:43.000000 mereja-0.0.4/mereja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 17:16:43.000000 mereja-0.0.4/mereja.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-04 17:16:43.630593 mereja-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-04 17:16:31.000000 mereja-0.0.4/setup.py
```

### Comparing `mereja-0.0.3/PKG-INFO` & `mereja-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: mereja
-Version: 0.0.3
-Home-page: https://github.com/wizkiye/mereja
-Author: Kidus
-Author-email: wizkiye@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # Mereja
 
 [![Python](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
 
 ## Description
 Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data, trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
 
@@ -32,15 +19,15 @@
 
 1. Clone this repository:
 
 ```bash
 # for latest version
 pip install git+https://github.com/your-username/your-repo-name.git
 # or 
-pip install mereja
+pip install mereja -U
 ```
 
 ## Usage
 
 ```bash
 mereja --help
 ```
@@ -78,18 +65,18 @@
   --path PATH, -pa PATH
                         Path to export file
 ```
 
 ## Examples
 
 <details>
-<summary>Without any options</summary>
+<summary>RUN without any options/args</summary>
 
 ```bash
-# Without any options
+# Running without any options/args
 mereja
 ```
 ![Made with VHS](https://vhs.charm.sh/vhs-3U79nZQbOZOCFYqxnIu0d0.gif)
 
 </details>
 
 <details>
@@ -183,15 +170,15 @@
 <details>
 <summary>Export to file</summary>
 
 ```bash
 # Export to file
 mereja --job --latest --export --path "jobs.json"
 
-# you can use the -e flag in any command to export to file i think :)
+# You can use the -e flag in commands to export data to a JSON file, I think.
 ```
 
 </details>
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `mereja-0.0.3/README.md` & `mereja-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: mereja
+Version: 0.0.4
+Home-page: https://github.com/wizkiye/mereja
+Author: Kidus
+Author-email: wizkiye@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 # Mereja
 
 [![Python](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
 
 ## Description
 Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data, trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
 
@@ -19,15 +32,15 @@
 
 1. Clone this repository:
 
 ```bash
 # for latest version
 pip install git+https://github.com/your-username/your-repo-name.git
 # or 
-pip install mereja
+pip install mereja -U
 ```
 
 ## Usage
 
 ```bash
 mereja --help
 ```
@@ -65,18 +78,18 @@
   --path PATH, -pa PATH
                         Path to export file
 ```
 
 ## Examples
 
 <details>
-<summary>Without any options</summary>
+<summary>RUN without any options/args</summary>
 
 ```bash
-# Without any options
+# Running without any options/args
 mereja
 ```
 ![Made with VHS](https://vhs.charm.sh/vhs-3U79nZQbOZOCFYqxnIu0d0.gif)
 
 </details>
 
 <details>
@@ -170,15 +183,15 @@
 <details>
 <summary>Export to file</summary>
 
 ```bash
 # Export to file
 mereja --job --latest --export --path "jobs.json"
 
-# you can use the -e flag in any command to export to file i think :)
+# You can use the -e flag in commands to export data to a JSON file, I think.
 ```
 
 </details>
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `mereja-0.0.3/mereja/constants.py` & `mereja-0.0.4/mereja/constants.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.3/mereja/functions/forex.py` & `mereja-0.0.4/mereja/functions/forex.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.3/mereja/functions/jobs.py` & `mereja-0.0.4/mereja/functions/jobs.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.3/mereja/functions/market.py` & `mereja-0.0.4/mereja/functions/market.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.3/mereja/functions/news.py` & `mereja-0.0.4/mereja/functions/news.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.3/mereja/functions/telebirr.py` & `mereja-0.0.4/mereja/functions/telebirr.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.3/mereja/main.py` & `mereja-0.0.4/mereja/main.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.3/mereja/ui/forex_table_ui.py` & `mereja-0.0.4/mereja/ui/forex_table_ui.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.3/mereja/ui/job_view_ui.py` & `mereja-0.0.4/mereja/ui/job_view_ui.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.3/mereja/ui/marketpalce_ui.py` & `mereja-0.0.4/mereja/ui/marketpalce_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from rich.align import Align
 from rich.console import Group
 from rich.layout import Layout
 from rich.live import Live
 from rich.panel import Panel
 from rich.table import Table
 
-from mereja.utils import make_qr, bold_numbers
+from mereja.utils import make_qr, bold_numbers, clean_emoji
 
 
 def make_layout() -> Layout:
     """Define the layout."""
     layout = Layout(name="root")
 
     layout.split(
@@ -52,21 +52,21 @@
     details.add_column(justify="left", ratio=1)
     details.add_row(
         f"[b]Description:[/b] ",
         f"[blue i]" + product.description.replace("<br>", " ").strip(),
     )
     details.add_row(
         f"[b]Location:[/b]",
-        f"[blue]:earth_africa: {', '.join(product.regions_display).strip()}[/blue]",
+        f"[blue]:earth_africa:{', '.join(product.regions_display).strip()}[/blue]",
     )
     details.add_row(
         f"[b]Posted:[/b] ",
         f"[blue b]:date: {product.date_created.strftime('%d %b %Y')}[/blue b]",
     )
-    details.add_row(f"[b]Views:[/b]", f"[blue b]:eye: {product.page_views}[/blue b]")
+    details.add_row(f"[b]Views:[/b]", f"[blue b]👀{product.page_views}[/blue b]")
     details.add_row(
         f"[b]Likes:[/b]", f"[blue b]:thumbsup: {product.fav_count}[/blue b]"
     )
     details.add_row(f"[b]Price:[/b]", f"[blue b]:dollar: {product.price} ETB[/blue b]")
     details.add_row(f"[b]Category:[/b]", f"[blue]{product.category_slug}[/blue]")
     if product.price_valuation:
         details.add_row(
@@ -95,15 +95,15 @@
         grid.add_column(justify="center", ratio=1)
         grid.add_row(self.title)
         return Panel(grid)
 
 
 def user_details(user: User) -> Align:
     return Align.center(
-        f"[b]Seller Name:[/b] [u blue]🙎 {user.name}[/u blue]\n"
+        f"[b]Seller Name:[/b] [u blue]🙎 {clean_emoji(user.name)}[/u blue]\n"
         f"[b]Phone Number:[/b] [blue]📞 {', '.join(user.phones)}[/blue]\n"
         f"[b]Email:[/b] [blue]📧 {user.email}[/blue]\n"
         f"[b]lastSeen:[/b] [blue]👀 {user.last_seen}[/blue]\n"
         f"[b]Registered at:[/b] [blue]📅 {user.user_registered}[/blue] [b]ago\n",
         vertical="middle",
     )
```

### Comparing `mereja-0.0.3/mereja/ui/news_view_ui.py` & `mereja-0.0.4/mereja/ui/news_view_ui.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.3/mereja/ui/transaction_table.py` & `mereja-0.0.4/mereja/ui/transaction_table.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.3/mereja/ui/widgets/header.py` & `mereja-0.0.4/mereja/ui/widgets/header.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.3/mereja/utils.py` & `mereja-0.0.4/mereja/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -156,7 +156,17 @@
 
     return run
 
 
 def no_ans_or_back(ans: str):
     if not ans:
         raise KeyboardInterrupt
+
+
+def clean_emoji(text: str) -> str:
+    return re.compile(
+        "[^\U00000000-\U0000d7ff\U0000e000-\U0000ffff]", flags=re.UNICODE
+    ).sub("", text)
+
+
+if __name__ == "__main__":
+    print(clean_emoji("hello 🔙"))
```

### Comparing `mereja-0.0.3/mereja.egg-info/PKG-INFO` & `mereja-0.0.4/mereja.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mereja
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/wizkiye/mereja
 Author: Kidus
 Author-email: wizkiye@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,15 +32,15 @@
 
 1. Clone this repository:
 
 ```bash
 # for latest version
 pip install git+https://github.com/your-username/your-repo-name.git
 # or 
-pip install mereja
+pip install mereja -U
 ```
 
 ## Usage
 
 ```bash
 mereja --help
 ```
@@ -78,18 +78,18 @@
   --path PATH, -pa PATH
                         Path to export file
 ```
 
 ## Examples
 
 <details>
-<summary>Without any options</summary>
+<summary>RUN without any options/args</summary>
 
 ```bash
-# Without any options
+# Running without any options/args
 mereja
 ```
 ![Made with VHS](https://vhs.charm.sh/vhs-3U79nZQbOZOCFYqxnIu0d0.gif)
 
 </details>
 
 <details>
@@ -183,15 +183,15 @@
 <details>
 <summary>Export to file</summary>
 
 ```bash
 # Export to file
 mereja --job --latest --export --path "jobs.json"
 
-# you can use the -e flag in any command to export to file i think :)
+# You can use the -e flag in commands to export data to a JSON file, I think.
 ```
 
 </details>
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `mereja-0.0.3/mereja.egg-info/SOURCES.txt` & `mereja-0.0.4/mereja.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mereja-0.0.3/setup.py` & `mereja-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_file(filename: str):
     with open(filename, encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="mereja",
-    version="0.0.3",
+    version="0.0.4",
     packages=find_packages(),
     url="https://github.com/wizkiye/mereja",
     license="MIT",
     author="Kidus",
     author_email="wizkiye@gmail.com",
     description="",
     install_requires=[
```

