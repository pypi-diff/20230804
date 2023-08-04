# Comparing `tmp/mereja-0.0.1.tar.gz` & `tmp/mereja-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mereja-0.0.1.tar", last modified: Fri Aug  4 14:52:54 2023, max compression
+gzip compressed data, was "mereja-0.0.2.tar", last modified: Fri Aug  4 15:50:30 2023, max compression
```

## Comparing `mereja-0.0.1.tar` & `mereja-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 14:52:54.159792 mereja-0.0.1/
--rw-rw-rw-   0        0        0     5097 2023-08-04 14:52:54.159792 mereja-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4767 2023-08-04 14:49:55.000000 mereja-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 14:52:54.129197 mereja-0.0.1/mereja/
--rw-rw-rw-   0        0        0       46 2023-08-02 18:18:00.000000 mereja-0.0.1/mereja/__init__.py
--rw-rw-rw-   0        0        0     1716 2023-08-03 15:13:30.000000 mereja-0.0.1/mereja/constants.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:52:54.151389 mereja-0.0.1/mereja/functions/
--rw-rw-rw-   0        0        0       50 2023-08-02 11:35:46.000000 mereja-0.0.1/mereja/functions/__init__.py
--rw-rw-rw-   0        0        0      919 2023-08-03 19:40:34.000000 mereja-0.0.1/mereja/functions/forex.py
--rw-rw-rw-   0        0        0     2602 2023-08-03 19:35:57.000000 mereja-0.0.1/mereja/functions/jobs.py
--rw-rw-rw-   0        0        0     3008 2023-08-03 19:50:55.000000 mereja-0.0.1/mereja/functions/market.py
--rw-rw-rw-   0        0        0     2474 2023-08-03 19:45:27.000000 mereja-0.0.1/mereja/functions/news.py
--rw-rw-rw-   0        0        0     1107 2023-08-03 20:28:40.000000 mereja-0.0.1/mereja/functions/telebirr.py
--rw-rw-rw-   0        0        0    11605 2023-08-04 14:28:52.000000 mereja-0.0.1/mereja/main.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:52:54.156386 mereja-0.0.1/mereja/ui/
--rw-rw-rw-   0        0        0      216 2023-08-02 14:55:57.000000 mereja-0.0.1/mereja/ui/__init__.py
--rw-rw-rw-   0        0        0     2572 2023-08-02 14:55:57.000000 mereja-0.0.1/mereja/ui/forex_table_ui.py
--rw-rw-rw-   0        0        0     2744 2023-08-04 12:56:43.000000 mereja-0.0.1/mereja/ui/job_view_ui.py
--rw-rw-rw-   0        0        0     4111 2023-08-04 08:14:56.000000 mereja-0.0.1/mereja/ui/marketpalce_ui.py
--rw-rw-rw-   0        0        0      764 2023-08-02 14:55:57.000000 mereja-0.0.1/mereja/ui/news_view_ui.py
--rw-rw-rw-   0        0        0     3131 2023-08-02 14:55:57.000000 mereja-0.0.1/mereja/ui/transaction_table.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:52:54.158781 mereja-0.0.1/mereja/ui/widgets/
--rw-rw-rw-   0        0        0       27 2023-08-01 08:02:11.000000 mereja-0.0.1/mereja/ui/widgets/__init__.py
--rw-rw-rw-   0        0        0     2679 2023-08-04 07:43:26.000000 mereja-0.0.1/mereja/ui/widgets/header.py
--rw-rw-rw-   0        0        0     3832 2023-08-03 19:20:41.000000 mereja-0.0.1/mereja/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:52:54.145282 mereja-0.0.1/mereja.egg-info/
--rw-rw-rw-   0        0        0     5097 2023-08-04 14:52:54.000000 mereja-0.0.1/mereja.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      659 2023-08-04 14:52:54.000000 mereja-0.0.1/mereja.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 14:52:54.000000 mereja-0.0.1/mereja.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-08-04 14:52:54.000000 mereja-0.0.1/mereja.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       91 2023-08-04 14:52:54.000000 mereja-0.0.1/mereja.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-04 14:52:54.000000 mereja-0.0.1/mereja.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      433 2023-08-04 14:52:54.164832 mereja-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      856 2023-08-04 14:52:40.000000 mereja-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:50:30.423201 mereja-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-08-04 15:50:30.423201 mereja-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-08-04 15:50:20.000000 mereja-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:50:30.419201 mereja-0.0.2/mereja/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:50:30.423201 mereja-0.0.2/mereja/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/functions/forex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/functions/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/functions/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/functions/news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/functions/telebirr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:50:30.423201 mereja-0.0.2/mereja/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/ui/forex_table_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/ui/job_view_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/ui/marketpalce_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/ui/news_view_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/ui/transaction_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:50:30.423201 mereja-0.0.2/mereja/ui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/ui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/ui/widgets/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-08-04 15:50:20.000000 mereja-0.0.2/mereja/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:50:30.423201 mereja-0.0.2/mereja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-08-04 15:50:30.000000 mereja-0.0.2/mereja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-04 15:50:30.000000 mereja-0.0.2/mereja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:50:30.000000 mereja-0.0.2/mereja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 15:50:30.000000 mereja-0.0.2/mereja.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-04 15:50:30.000000 mereja-0.0.2/mereja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 15:50:30.000000 mereja-0.0.2/mereja.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-04 15:50:30.423201 mereja-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-04 15:50:20.000000 mereja-0.0.2/setup.py
```

### Comparing `mereja-0.0.1/PKG-INFO` & `mereja-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,190 +1,191 @@
-Metadata-Version: 2.1
-Name: mereja
-Version: 0.0.1
-Home-page: 
-Author: Kidus
-Author-email: wizkiye@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
-# Mereja
-
-[![Python](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
-
-## Description
-Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data, trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
-
-## Features
-
-- Scrape and display the latest news articles.
-- Browse and search for job opportunities.
-- Access and visualize forex data.
-- Find trending products on marketplaces.
-- Retrieve telebirr transaction details.
-- Command-line interface for easy interaction.
-- Text-based User Interface (TUI) for interactive browsing.
-
-## Installation
-
-1. Clone this repository:
-
-```bash
-# for latest version
-pip install git+https://github.com/your-username/your-repo-name.git
-# or 
-pip install mereja
-```
-
-## Usage
-
-```bash
-mereja --help
-```
-
-## Options
-
-```bash
-usage: mereja [-h] [--job] [--marketplace] [--telebirr] [--forex] [--news] [--latest] [--trending]
-              [--transaction TRANSACTION] [--live] [--page PAGE] [--limit LIMIT] [--search SEARCH] [--export]
-              [--path PATH]
-
-Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User
-Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data,
-trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality
-for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
-
-options:
-  -h, --help            show this help message and exit
-  --job, -j             Jobs
-  --marketplace, -m     Marketplace
-  --telebirr, -tb       Telebirr
-  --forex, -f           Forex
-  --news, -n            News
-  --latest, -lt         Get latest jobs.
-  --trending, -t        Get trending products
-  --transaction TRANSACTION, -tx TRANSACTION
-                        Telebirr Transaction ID
-  --live, -lv           Watch Live forex
-  --page PAGE, -p PAGE  Page number
-  --limit LIMIT, -l LIMIT
-                        Limit number
-  --search SEARCH, -s SEARCH
-                        Search for a job/product/news
-  --export, -e          Export to file
-  --path PATH, -pa PATH
-                        Path to export file
-```
-
-## Examples
-<details>
-<summary>Get latest jobs</summary>
-
-```bash
-# Get latest jobs
-mereja --job --latest
-```
-![Made with VHS](https://vhs.charm.sh/vhs-6OYIlBEo1QGqbBXxsF9kCb.gif)
-
-</details>
-
-<details>
-<summary>Get trending products</summary>
-
-```bash
-# Get trending products
-mereja --marketplace --trending
-```
-![Made with VHS](https://vhs.charm.sh/vhs-6OV1lF4iTx1BBfXVMoyBpe.gif)
-
-</details>
-
-<details>
-<summary>Get telebirr transaction details</summary>
-
-```bash
-# Get telebirr transaction details
-mereja --telebirr --transaction 123456789
-```
-![Made with VHS](https://vhs.charm.sh/vhs-7r8opSediv95hSYrbrDkqf.gif)
-
-</details>
-
-<details>
-<summary>Get live forex data</summary>
-
-```bash
-# Get live forex data
-mereja --forex --live
-```
-![Made with VHS](https://vhs.charm.sh/vhs-2bwN1U2auQbepuc3tvJ7H.gif)
-</details>
-
-<details>
-<summary>Get latest news</summary>
-
-```bash
-# Get latest news
-mereja --news --latest
-```
-![Made with VHS](https://vhs.charm.sh/vhs-5yikXD3R1aA7EsiU0NVt2H.gif)
-
-</details>
-
-<details>
-<summary>Search for jobs</summary>
-
-```bash
-# Search for jobs
-mereja --job --search "IT"
-```
-![Made with VHS](https://vhs.charm.sh/vhs-8hoM1DhnzctU0moJqk994.gif)
-
-</details>
-
-<details>
-<summary>Search for products</summary>
-
-```bash
-# Search for products
-mereja --marketplace --search "s23"
-```
-![Made with VHS](https://vhs.charm.sh/vhs-bNr6qDbaOnV6afVAaK96s.gif)
-
-</details>
-
-<details>
-<summary>Search for news</summary>
-
-```bash
-# Search for news
-mereja --news --search "ራሽያ"
-```
- ![Made with VHS](https://vhs.charm.sh/vhs-3xJSIxwi4g5OS48lxdDFtP.gif)
-
-
-</details>
-
-<details>
-<summary>Export to file</summary>
-
-```bash
-# Export to file
-mereja --job --latest --export --path "jobs.json"
-
-# you can use the -e flag in any command to export to file i think :)
-```
-
-</details>
-
-## Contributing
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-## License
-[MIT](https://choosealicense.com/licenses/mit/)
-
-
-
-
+Metadata-Version: 2.1
+Name: mereja
+Version: 0.0.2
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
+# Mereja
+
+[![Python](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
+
+## Description
+Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data, trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
+
+## Features
+
+- Scrape and display the latest news articles.
+- Browse and search for job opportunities.
+- Access and visualize forex data.
+- Find trending products on marketplaces.
+- Retrieve telebirr transaction details.
+- Command-line interface for easy interaction.
+- Text-based User Interface (TUI) for interactive browsing.
+
+## Installation
+
+1. Clone this repository:
+
+```bash
+# for latest version
+pip install git+https://github.com/your-username/your-repo-name.git
+# or 
+pip install mereja
+```
+
+## Usage
+
+```bash
+mereja --help
+```
+
+## Options
+
+```bash
+usage: mereja [-h] [--job] [--marketplace] [--telebirr] [--forex] [--news] [--latest] [--trending]
+              [--transaction TRANSACTION] [--live] [--page PAGE] [--limit LIMIT] [--search SEARCH] [--export]
+              [--path PATH]
+
+Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User
+Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data,
+trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality
+for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
+
+options:
+  -h, --help            show this help message and exit
+  --job, -j             Jobs
+  --marketplace, -m     Marketplace
+  --telebirr, -tb       Telebirr
+  --forex, -f           Forex
+  --news, -n            News
+  --latest, -lt         Get latest jobs.
+  --trending, -t        Get trending products
+  --transaction TRANSACTION, -tx TRANSACTION
+                        Telebirr Transaction ID
+  --live, -lv           Watch Live forex
+  --page PAGE, -p PAGE  Page number
+  --limit LIMIT, -l LIMIT
+                        Limit number
+  --search SEARCH, -s SEARCH
+                        Search for a job/product/news
+  --export, -e          Export to file
+  --path PATH, -pa PATH
+                        Path to export file
+```
+
+## Examples
+<details>
+<summary>Get latest jobs</summary>
+
+```bash
+# Get latest jobs
+mereja --job --latest
+```
+![Made with VHS](https://vhs.charm.sh/vhs-6OYIlBEo1QGqbBXxsF9kCb.gif)
+
+</details>
+
+<details>
+<summary>Get trending products</summary>
+
+```bash
+# Get trending products
+mereja --marketplace --trending
+```
+![Made with VHS](https://vhs.charm.sh/vhs-6OV1lF4iTx1BBfXVMoyBpe.gif)
+
+</details>
+
+<details>
+<summary>Get telebirr transaction details</summary>
+
+```bash
+# Get telebirr transaction details
+mereja --telebirr --transaction 123456789
+```
+![Made with VHS](https://vhs.charm.sh/vhs-7r8opSediv95hSYrbrDkqf.gif)
+
+</details>
+
+<details>
+<summary>Get live forex data</summary>
+
+```bash
+# Get live forex data
+mereja --forex --live
+```
+![Made with VHS](https://vhs.charm.sh/vhs-2bwN1U2auQbepuc3tvJ7H.gif)
+</details>
+
+<details>
+<summary>Get latest news</summary>
+
+```bash
+# Get latest news
+mereja --news --latest
+```
+![Made with VHS](https://vhs.charm.sh/vhs-5yikXD3R1aA7EsiU0NVt2H.gif)
+
+</details>
+
+<details>
+<summary>Search for jobs</summary>
+
+```bash
+# Search for jobs
+mereja --job --search "IT"
+```
+![Made with VHS](https://vhs.charm.sh/vhs-8hoM1DhnzctU0moJqk994.gif)
+
+</details>
+
+<details>
+<summary>Search for products</summary>
+
+```bash
+# Search for products
+mereja --marketplace --search "s23"
+```
+![Made with VHS](https://vhs.charm.sh/vhs-bNr6qDbaOnV6afVAaK96s.gif)
+
+</details>
+
+<details>
+<summary>Search for news</summary>
+
+```bash
+# Search for news
+mereja --news --search "ራሽያ"
+```
+ ![Made with VHS](https://vhs.charm.sh/vhs-3xJSIxwi4g5OS48lxdDFtP.gif)
+
+
+</details>
+
+<details>
+<summary>Export to file</summary>
+
+```bash
+# Export to file
+mereja --job --latest --export --path "jobs.json"
+
+# you can use the -e flag in any command to export to file i think :)
+```
+
+</details>
+
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+## License
+[MIT](https://choosealicense.com/licenses/mit/)
+
+
+
+
```

### Comparing `mereja-0.0.1/README.md` & `mereja-0.0.2/mereja.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,178 +1,191 @@
-# Mereja
-
-[![Python](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
-
-## Description
-Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data, trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
-
-## Features
-
-- Scrape and display the latest news articles.
-- Browse and search for job opportunities.
-- Access and visualize forex data.
-- Find trending products on marketplaces.
-- Retrieve telebirr transaction details.
-- Command-line interface for easy interaction.
-- Text-based User Interface (TUI) for interactive browsing.
-
-## Installation
-
-1. Clone this repository:
-
-```bash
-# for latest version
-pip install git+https://github.com/your-username/your-repo-name.git
-# or 
-pip install mereja
-```
-
-## Usage
-
-```bash
-mereja --help
-```
-
-## Options
-
-```bash
-usage: mereja [-h] [--job] [--marketplace] [--telebirr] [--forex] [--news] [--latest] [--trending]
-              [--transaction TRANSACTION] [--live] [--page PAGE] [--limit LIMIT] [--search SEARCH] [--export]
-              [--path PATH]
-
-Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User
-Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data,
-trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality
-for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
-
-options:
-  -h, --help            show this help message and exit
-  --job, -j             Jobs
-  --marketplace, -m     Marketplace
-  --telebirr, -tb       Telebirr
-  --forex, -f           Forex
-  --news, -n            News
-  --latest, -lt         Get latest jobs.
-  --trending, -t        Get trending products
-  --transaction TRANSACTION, -tx TRANSACTION
-                        Telebirr Transaction ID
-  --live, -lv           Watch Live forex
-  --page PAGE, -p PAGE  Page number
-  --limit LIMIT, -l LIMIT
-                        Limit number
-  --search SEARCH, -s SEARCH
-                        Search for a job/product/news
-  --export, -e          Export to file
-  --path PATH, -pa PATH
-                        Path to export file
-```
-
-## Examples
-<details>
-<summary>Get latest jobs</summary>
-
-```bash
-# Get latest jobs
-mereja --job --latest
-```
-![Made with VHS](https://vhs.charm.sh/vhs-6OYIlBEo1QGqbBXxsF9kCb.gif)
-
-</details>
-
-<details>
-<summary>Get trending products</summary>
-
-```bash
-# Get trending products
-mereja --marketplace --trending
-```
-![Made with VHS](https://vhs.charm.sh/vhs-6OV1lF4iTx1BBfXVMoyBpe.gif)
-
-</details>
-
-<details>
-<summary>Get telebirr transaction details</summary>
-
-```bash
-# Get telebirr transaction details
-mereja --telebirr --transaction 123456789
-```
-![Made with VHS](https://vhs.charm.sh/vhs-7r8opSediv95hSYrbrDkqf.gif)
-
-</details>
-
-<details>
-<summary>Get live forex data</summary>
-
-```bash
-# Get live forex data
-mereja --forex --live
-```
-![Made with VHS](https://vhs.charm.sh/vhs-2bwN1U2auQbepuc3tvJ7H.gif)
-</details>
-
-<details>
-<summary>Get latest news</summary>
-
-```bash
-# Get latest news
-mereja --news --latest
-```
-![Made with VHS](https://vhs.charm.sh/vhs-5yikXD3R1aA7EsiU0NVt2H.gif)
-
-</details>
-
-<details>
-<summary>Search for jobs</summary>
-
-```bash
-# Search for jobs
-mereja --job --search "IT"
-```
-![Made with VHS](https://vhs.charm.sh/vhs-8hoM1DhnzctU0moJqk994.gif)
-
-</details>
-
-<details>
-<summary>Search for products</summary>
-
-```bash
-# Search for products
-mereja --marketplace --search "s23"
-```
-![Made with VHS](https://vhs.charm.sh/vhs-bNr6qDbaOnV6afVAaK96s.gif)
-
-</details>
-
-<details>
-<summary>Search for news</summary>
-
-```bash
-# Search for news
-mereja --news --search "ራሽያ"
-```
- ![Made with VHS](https://vhs.charm.sh/vhs-3xJSIxwi4g5OS48lxdDFtP.gif)
-
-
-</details>
-
-<details>
-<summary>Export to file</summary>
-
-```bash
-# Export to file
-mereja --job --latest --export --path "jobs.json"
-
-# you can use the -e flag in any command to export to file i think :)
-```
-
-</details>
-
-## Contributing
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-## License
-[MIT](https://choosealicense.com/licenses/mit/)
-
-
-
-
+Metadata-Version: 2.1
+Name: mereja
+Version: 0.0.2
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
+# Mereja
+
+[![Python](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
+
+## Description
+Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data, trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
+
+## Features
+
+- Scrape and display the latest news articles.
+- Browse and search for job opportunities.
+- Access and visualize forex data.
+- Find trending products on marketplaces.
+- Retrieve telebirr transaction details.
+- Command-line interface for easy interaction.
+- Text-based User Interface (TUI) for interactive browsing.
+
+## Installation
+
+1. Clone this repository:
+
+```bash
+# for latest version
+pip install git+https://github.com/your-username/your-repo-name.git
+# or 
+pip install mereja
+```
+
+## Usage
+
+```bash
+mereja --help
+```
+
+## Options
+
+```bash
+usage: mereja [-h] [--job] [--marketplace] [--telebirr] [--forex] [--news] [--latest] [--trending]
+              [--transaction TRANSACTION] [--live] [--page PAGE] [--limit LIMIT] [--search SEARCH] [--export]
+              [--path PATH]
+
+Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User
+Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data,
+trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality
+for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
+
+options:
+  -h, --help            show this help message and exit
+  --job, -j             Jobs
+  --marketplace, -m     Marketplace
+  --telebirr, -tb       Telebirr
+  --forex, -f           Forex
+  --news, -n            News
+  --latest, -lt         Get latest jobs.
+  --trending, -t        Get trending products
+  --transaction TRANSACTION, -tx TRANSACTION
+                        Telebirr Transaction ID
+  --live, -lv           Watch Live forex
+  --page PAGE, -p PAGE  Page number
+  --limit LIMIT, -l LIMIT
+                        Limit number
+  --search SEARCH, -s SEARCH
+                        Search for a job/product/news
+  --export, -e          Export to file
+  --path PATH, -pa PATH
+                        Path to export file
+```
+
+## Examples
+<details>
+<summary>Get latest jobs</summary>
+
+```bash
+# Get latest jobs
+mereja --job --latest
+```
+![Made with VHS](https://vhs.charm.sh/vhs-6OYIlBEo1QGqbBXxsF9kCb.gif)
+
+</details>
+
+<details>
+<summary>Get trending products</summary>
+
+```bash
+# Get trending products
+mereja --marketplace --trending
+```
+![Made with VHS](https://vhs.charm.sh/vhs-6OV1lF4iTx1BBfXVMoyBpe.gif)
+
+</details>
+
+<details>
+<summary>Get telebirr transaction details</summary>
+
+```bash
+# Get telebirr transaction details
+mereja --telebirr --transaction 123456789
+```
+![Made with VHS](https://vhs.charm.sh/vhs-7r8opSediv95hSYrbrDkqf.gif)
+
+</details>
+
+<details>
+<summary>Get live forex data</summary>
+
+```bash
+# Get live forex data
+mereja --forex --live
+```
+![Made with VHS](https://vhs.charm.sh/vhs-2bwN1U2auQbepuc3tvJ7H.gif)
+</details>
+
+<details>
+<summary>Get latest news</summary>
+
+```bash
+# Get latest news
+mereja --news --latest
+```
+![Made with VHS](https://vhs.charm.sh/vhs-5yikXD3R1aA7EsiU0NVt2H.gif)
+
+</details>
+
+<details>
+<summary>Search for jobs</summary>
+
+```bash
+# Search for jobs
+mereja --job --search "IT"
+```
+![Made with VHS](https://vhs.charm.sh/vhs-8hoM1DhnzctU0moJqk994.gif)
+
+</details>
+
+<details>
+<summary>Search for products</summary>
+
+```bash
+# Search for products
+mereja --marketplace --search "s23"
+```
+![Made with VHS](https://vhs.charm.sh/vhs-bNr6qDbaOnV6afVAaK96s.gif)
+
+</details>
+
+<details>
+<summary>Search for news</summary>
+
+```bash
+# Search for news
+mereja --news --search "ራሽያ"
+```
+ ![Made with VHS](https://vhs.charm.sh/vhs-3xJSIxwi4g5OS48lxdDFtP.gif)
+
+
+</details>
+
+<details>
+<summary>Export to file</summary>
+
+```bash
+# Export to file
+mereja --job --latest --export --path "jobs.json"
+
+# you can use the -e flag in any command to export to file i think :)
+```
+
+</details>
+
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+## License
+[MIT](https://choosealicense.com/licenses/mit/)
+
+
+
+
```

### Comparing `mereja-0.0.1/mereja/constants.py` & `mereja-0.0.2/mereja/constants.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.1/mereja/functions/jobs.py` & `mereja-0.0.2/mereja/functions/jobs.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.1/mereja/functions/news.py` & `mereja-0.0.2/mereja/functions/news.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.1/mereja/functions/telebirr.py` & `mereja-0.0.2/mereja/functions/telebirr.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.1/mereja/main.py` & `mereja-0.0.2/mereja/main.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.1/mereja/ui/forex_table_ui.py` & `mereja-0.0.2/mereja/ui/forex_table_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     table = Table(
         show_header=True,
         header_style="bold magenta",
         title=title,
         title_style="bold green",
     )
     table.add_column("Currency")
-    table.add_column("Buy", justify="right")
-    table.add_column("Sell", justify="right")
+    table.add_column("Buying RATE", justify="right")
+    table.add_column("Selling RATE", justify="right")
     for f in forex:
         table.add_row(
             f'[blue]{f["currency"]}', f'[cyan]{f["buy"]} ETB', f'[green]{f["sell"]} ETB'
         )
     return table
```

### Comparing `mereja-0.0.1/mereja/ui/job_view_ui.py` & `mereja-0.0.2/mereja/ui/job_view_ui.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.1/mereja/ui/marketpalce_ui.py` & `mereja-0.0.2/mereja/ui/marketpalce_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,25 +48,25 @@
             f"[b]{attr.name}[/b]",
             f"[i blue]{attr.value}[/i blue]",
         )
     details = Table.grid()
     details.add_column(justify="left", ratio=1)
     details.add_row(
         f"[b]Description:[/b] ",
-        f"[blue i]" + product.description.replace("<br>", " "),
+        f"[blue i]" + product.description.replace("<br>", " ").strip(),
     )
     details.add_row(
         f"[b]Location:[/b]",
-        f"[blue]:earth_africa: {', '.join(product.regions_display)}[/blue]",
+        f"[blue]:earth_africa: {', '.join(product.regions_display).strip()}[/blue]",
     )
     details.add_row(
         f"[b]Posted:[/b] ",
         f"[blue b]:date: {product.date_created.strftime('%d %b %Y')}[/blue b]",
     )
-    details.add_row(f"[b]Views:[/b]", f"[blue b]:eye:  {product.page_views}[/blue b]")
+    details.add_row(f"[b]Views:[/b]", f"[blue b]:eye: {product.page_views}[/blue b]")
     details.add_row(
         f"[b]Likes:[/b]", f"[blue b]:thumbsup: {product.fav_count}[/blue b]"
     )
     details.add_row(f"[b]Price:[/b]", f"[blue b]:dollar: {product.price} ETB[/blue b]")
     details.add_row(f"[b]Category:[/b]", f"[blue]{product.category_slug}[/blue]")
     if product.price_valuation:
         details.add_row(
```

### Comparing `mereja-0.0.1/mereja/ui/news_view_ui.py` & `mereja-0.0.2/mereja/ui/news_view_ui.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from markdownify import markdownify as md
-from pyEthioNews.providers.voa import VoaNewsDetail
-from textual.app import App, ComposeResult
-from textual.binding import Binding
-from textual.widgets import MarkdownViewer, Footer
-
-from mereja.ui.widgets import Header
-
-
-class NewsView(App):
-    def __init__(self, news: VoaNewsDetail = None):
-        self.news = news
-        super().__init__()
-
-    BINDINGS = [
-        Binding("q", "quit", "Quit"),
-    ]
-
-    def compose(self) -> ComposeResult:
-        yield Header(show_clock=True)
-        yield MarkdownViewer(
-            f"# {self.news.title}\n![image info]({self.news.image})"
-            + md(self.news.html),
-            show_table_of_contents=False,
-        )
-        yield Footer()
+from markdownify import markdownify as md
+from pyEthioNews.providers.voa import VoaNewsDetail
+from textual.app import App, ComposeResult
+from textual.binding import Binding
+from textual.widgets import MarkdownViewer, Footer
+
+from mereja.ui.widgets import Header
+
+
+class NewsView(App):
+    def __init__(self, news: VoaNewsDetail = None):
+        self.news = news
+        super().__init__()
+
+    BINDINGS = [
+        Binding("q", "quit", "Quit"),
+    ]
+
+    def compose(self) -> ComposeResult:
+        yield Header(show_clock=True)
+        yield MarkdownViewer(
+            f"# {self.news.title}\n![image info]({self.news.image})"
+            + md(self.news.html),
+            show_table_of_contents=False,
+        )
+        yield Footer()
```

### Comparing `mereja-0.0.1/mereja/ui/widgets/header.py` & `mereja-0.0.2/mereja/ui/widgets/header.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-from datetime import datetime
-
-from rich.text import Text
-from textual import events
-from textual.app import RenderResult
-from textual.events import Mount
-from textual.reactive import Reactive
-from textual.widget import Widget
-
-
-class HeaderIcon(Widget):
-    def __init__(self, icon: str = "📝") -> None:
-        super().__init__()
-        self.icon = icon
-
-    DEFAULT_CSS = """
-    HeaderIcon {
-        dock: left;
-        padding: 0 1;
-        width: 8;
-        content-align: left middle;
-    }
-    """
-
-    def render(self) -> RenderResult:
-        return self.icon
-
-
-class HeaderClockSpace(Widget):
-    DEFAULT_CSS = """
-    HeaderClockSpace {
-        dock: right;
-        width: 10;
-        padding: 0 1;
-    }
-    """
-
-    def render(self) -> RenderResult:
-        return ""
-
-
-class HeaderClock(HeaderClockSpace):
-    DEFAULT_CSS = """
-    HeaderClock {
-        background: $foreground-darken-1 5%;
-        color: $text;
-        text-opacity: 85%;
-        content-align: center middle;
-    }
-    """
-
-    def _on_mount(self, _: Mount) -> None:
-        self.set_interval(1, callback=self.refresh, name=f"update header clock")
-
-    def render(self) -> RenderResult:
-        return Text(datetime.now().time().strftime("%X"))
-
-
-class HeaderTitle(Widget):
-    def __init__(self, text: str) -> None:
-        super().__init__()
-        self.text = text
-
-    DEFAULT_CSS = """
-    HeaderTitle {
-        content-align: center middle;
-        width: 100%;
-    }
-    """
-
-    def render(self) -> RenderResult:
-        text = Text(self.text, no_wrap=True, overflow="ellipsis", style="bold blue")
-        return text
-
-
-class Header(Widget):
-    DEFAULT_CSS = """
-    Header {
-        dock: top;
-        width: 100%;
-        background: $foreground 5%;
-        color: $text;
-        height: 1;
-    }
-    Header.-tall {
-        height: 3;
-    }
-    """
-
-    DEFAULT_CLASSES = ""
-
-    tall: Reactive[bool] = Reactive(False)
-
-    def __init__(
-        self,
-        show_clock: bool = False,
-        title: str = "</> with ❤️ by @wizkiye",
-        *,
-        classes: str | None = None,
-        id: str | None = None,
-    ):
-        super().__init__(classes=classes, id=id)
-        self._show_clock = show_clock
-        self.title = title
-
-    def compose(self):
-        yield HeaderIcon()
-        yield HeaderTitle(self.title)
-        yield HeaderClock() if self._show_clock else HeaderClockSpace()
-
-    def watch_tall(self, tall: bool) -> None:
-        self.set_class(tall, "-tall")
-
-    def _on_click(self, event: events.Click):
-        self.toggle_class("-tall")
+from datetime import datetime
+
+from rich.text import Text
+from textual import events
+from textual.app import RenderResult
+from textual.events import Mount
+from textual.reactive import Reactive
+from textual.widget import Widget
+
+
+class HeaderIcon(Widget):
+    def __init__(self, icon: str = "📝") -> None:
+        super().__init__()
+        self.icon = icon
+
+    DEFAULT_CSS = """
+    HeaderIcon {
+        dock: left;
+        padding: 0 1;
+        width: 8;
+        content-align: left middle;
+    }
+    """
+
+    def render(self) -> RenderResult:
+        return self.icon
+
+
+class HeaderClockSpace(Widget):
+    DEFAULT_CSS = """
+    HeaderClockSpace {
+        dock: right;
+        width: 10;
+        padding: 0 1;
+    }
+    """
+
+    def render(self) -> RenderResult:
+        return ""
+
+
+class HeaderClock(HeaderClockSpace):
+    DEFAULT_CSS = """
+    HeaderClock {
+        background: $foreground-darken-1 5%;
+        color: $text;
+        text-opacity: 85%;
+        content-align: center middle;
+    }
+    """
+
+    def _on_mount(self, _: Mount) -> None:
+        self.set_interval(1, callback=self.refresh, name=f"update header clock")
+
+    def render(self) -> RenderResult:
+        return Text(datetime.now().time().strftime("%X"))
+
+
+class HeaderTitle(Widget):
+    def __init__(self, text: str) -> None:
+        super().__init__()
+        self.text = text
+
+    DEFAULT_CSS = """
+    HeaderTitle {
+        content-align: center middle;
+        width: 100%;
+    }
+    """
+
+    def render(self) -> RenderResult:
+        text = Text(self.text, no_wrap=True, overflow="ellipsis", style="bold blue")
+        return text
+
+
+class Header(Widget):
+    DEFAULT_CSS = """
+    Header {
+        dock: top;
+        width: 100%;
+        background: $foreground 5%;
+        color: $text;
+        height: 1;
+    }
+    Header.-tall {
+        height: 3;
+    }
+    """
+
+    DEFAULT_CLASSES = ""
+
+    tall: Reactive[bool] = Reactive(False)
+
+    def __init__(
+        self,
+        show_clock: bool = False,
+        title: str = "</> with ❤️ by @wizkiye",
+        *,
+        classes: str | None = None,
+        id: str | None = None,
+    ):
+        super().__init__(classes=classes, id=id)
+        self._show_clock = show_clock
+        self.title = title
+
+    def compose(self):
+        yield HeaderIcon()
+        yield HeaderTitle(self.title)
+        yield HeaderClock() if self._show_clock else HeaderClockSpace()
+
+    def watch_tall(self, tall: bool) -> None:
+        self.set_class(tall, "-tall")
+
+    def _on_click(self, event: events.Click):
+        self.toggle_class("-tall")
```

### Comparing `mereja-0.0.1/mereja/utils.py` & `mereja-0.0.2/mereja/utils.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.1/mereja.egg-info/PKG-INFO` & `mereja-0.0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,190 +1,178 @@
-Metadata-Version: 2.1
-Name: mereja
-Version: 0.0.1
-Home-page: 
-Author: Kidus
-Author-email: wizkiye@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
-# Mereja
-
-[![Python](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
-
-## Description
-Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data, trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
-
-## Features
-
-- Scrape and display the latest news articles.
-- Browse and search for job opportunities.
-- Access and visualize forex data.
-- Find trending products on marketplaces.
-- Retrieve telebirr transaction details.
-- Command-line interface for easy interaction.
-- Text-based User Interface (TUI) for interactive browsing.
-
-## Installation
-
-1. Clone this repository:
-
-```bash
-# for latest version
-pip install git+https://github.com/your-username/your-repo-name.git
-# or 
-pip install mereja
-```
-
-## Usage
-
-```bash
-mereja --help
-```
-
-## Options
-
-```bash
-usage: mereja [-h] [--job] [--marketplace] [--telebirr] [--forex] [--news] [--latest] [--trending]
-              [--transaction TRANSACTION] [--live] [--page PAGE] [--limit LIMIT] [--search SEARCH] [--export]
-              [--path PATH]
-
-Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User
-Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data,
-trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality
-for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
-
-options:
-  -h, --help            show this help message and exit
-  --job, -j             Jobs
-  --marketplace, -m     Marketplace
-  --telebirr, -tb       Telebirr
-  --forex, -f           Forex
-  --news, -n            News
-  --latest, -lt         Get latest jobs.
-  --trending, -t        Get trending products
-  --transaction TRANSACTION, -tx TRANSACTION
-                        Telebirr Transaction ID
-  --live, -lv           Watch Live forex
-  --page PAGE, -p PAGE  Page number
-  --limit LIMIT, -l LIMIT
-                        Limit number
-  --search SEARCH, -s SEARCH
-                        Search for a job/product/news
-  --export, -e          Export to file
-  --path PATH, -pa PATH
-                        Path to export file
-```
-
-## Examples
-<details>
-<summary>Get latest jobs</summary>
-
-```bash
-# Get latest jobs
-mereja --job --latest
-```
-![Made with VHS](https://vhs.charm.sh/vhs-6OYIlBEo1QGqbBXxsF9kCb.gif)
-
-</details>
-
-<details>
-<summary>Get trending products</summary>
-
-```bash
-# Get trending products
-mereja --marketplace --trending
-```
-![Made with VHS](https://vhs.charm.sh/vhs-6OV1lF4iTx1BBfXVMoyBpe.gif)
-
-</details>
-
-<details>
-<summary>Get telebirr transaction details</summary>
-
-```bash
-# Get telebirr transaction details
-mereja --telebirr --transaction 123456789
-```
-![Made with VHS](https://vhs.charm.sh/vhs-7r8opSediv95hSYrbrDkqf.gif)
-
-</details>
-
-<details>
-<summary>Get live forex data</summary>
-
-```bash
-# Get live forex data
-mereja --forex --live
-```
-![Made with VHS](https://vhs.charm.sh/vhs-2bwN1U2auQbepuc3tvJ7H.gif)
-</details>
-
-<details>
-<summary>Get latest news</summary>
-
-```bash
-# Get latest news
-mereja --news --latest
-```
-![Made with VHS](https://vhs.charm.sh/vhs-5yikXD3R1aA7EsiU0NVt2H.gif)
-
-</details>
-
-<details>
-<summary>Search for jobs</summary>
-
-```bash
-# Search for jobs
-mereja --job --search "IT"
-```
-![Made with VHS](https://vhs.charm.sh/vhs-8hoM1DhnzctU0moJqk994.gif)
-
-</details>
-
-<details>
-<summary>Search for products</summary>
-
-```bash
-# Search for products
-mereja --marketplace --search "s23"
-```
-![Made with VHS](https://vhs.charm.sh/vhs-bNr6qDbaOnV6afVAaK96s.gif)
-
-</details>
-
-<details>
-<summary>Search for news</summary>
-
-```bash
-# Search for news
-mereja --news --search "ራሽያ"
-```
- ![Made with VHS](https://vhs.charm.sh/vhs-3xJSIxwi4g5OS48lxdDFtP.gif)
-
-
-</details>
-
-<details>
-<summary>Export to file</summary>
-
-```bash
-# Export to file
-mereja --job --latest --export --path "jobs.json"
-
-# you can use the -e flag in any command to export to file i think :)
-```
-
-</details>
-
-## Contributing
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-## License
-[MIT](https://choosealicense.com/licenses/mit/)
-
-
-
-
+# Mereja
+
+[![Python](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
+
+## Description
+Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data, trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
+
+## Features
+
+- Scrape and display the latest news articles.
+- Browse and search for job opportunities.
+- Access and visualize forex data.
+- Find trending products on marketplaces.
+- Retrieve telebirr transaction details.
+- Command-line interface for easy interaction.
+- Text-based User Interface (TUI) for interactive browsing.
+
+## Installation
+
+1. Clone this repository:
+
+```bash
+# for latest version
+pip install git+https://github.com/your-username/your-repo-name.git
+# or 
+pip install mereja
+```
+
+## Usage
+
+```bash
+mereja --help
+```
+
+## Options
+
+```bash
+usage: mereja [-h] [--job] [--marketplace] [--telebirr] [--forex] [--news] [--latest] [--trending]
+              [--transaction TRANSACTION] [--live] [--page PAGE] [--limit LIMIT] [--search SEARCH] [--export]
+              [--path PATH]
+
+Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User
+Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data,
+trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality
+for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
+
+options:
+  -h, --help            show this help message and exit
+  --job, -j             Jobs
+  --marketplace, -m     Marketplace
+  --telebirr, -tb       Telebirr
+  --forex, -f           Forex
+  --news, -n            News
+  --latest, -lt         Get latest jobs.
+  --trending, -t        Get trending products
+  --transaction TRANSACTION, -tx TRANSACTION
+                        Telebirr Transaction ID
+  --live, -lv           Watch Live forex
+  --page PAGE, -p PAGE  Page number
+  --limit LIMIT, -l LIMIT
+                        Limit number
+  --search SEARCH, -s SEARCH
+                        Search for a job/product/news
+  --export, -e          Export to file
+  --path PATH, -pa PATH
+                        Path to export file
+```
+
+## Examples
+<details>
+<summary>Get latest jobs</summary>
+
+```bash
+# Get latest jobs
+mereja --job --latest
+```
+![Made with VHS](https://vhs.charm.sh/vhs-6OYIlBEo1QGqbBXxsF9kCb.gif)
+
+</details>
+
+<details>
+<summary>Get trending products</summary>
+
+```bash
+# Get trending products
+mereja --marketplace --trending
+```
+![Made with VHS](https://vhs.charm.sh/vhs-6OV1lF4iTx1BBfXVMoyBpe.gif)
+
+</details>
+
+<details>
+<summary>Get telebirr transaction details</summary>
+
+```bash
+# Get telebirr transaction details
+mereja --telebirr --transaction 123456789
+```
+![Made with VHS](https://vhs.charm.sh/vhs-7r8opSediv95hSYrbrDkqf.gif)
+
+</details>
+
+<details>
+<summary>Get live forex data</summary>
+
+```bash
+# Get live forex data
+mereja --forex --live
+```
+![Made with VHS](https://vhs.charm.sh/vhs-2bwN1U2auQbepuc3tvJ7H.gif)
+</details>
+
+<details>
+<summary>Get latest news</summary>
+
+```bash
+# Get latest news
+mereja --news --latest
+```
+![Made with VHS](https://vhs.charm.sh/vhs-5yikXD3R1aA7EsiU0NVt2H.gif)
+
+</details>
+
+<details>
+<summary>Search for jobs</summary>
+
+```bash
+# Search for jobs
+mereja --job --search "IT"
+```
+![Made with VHS](https://vhs.charm.sh/vhs-8hoM1DhnzctU0moJqk994.gif)
+
+</details>
+
+<details>
+<summary>Search for products</summary>
+
+```bash
+# Search for products
+mereja --marketplace --search "s23"
+```
+![Made with VHS](https://vhs.charm.sh/vhs-bNr6qDbaOnV6afVAaK96s.gif)
+
+</details>
+
+<details>
+<summary>Search for news</summary>
+
+```bash
+# Search for news
+mereja --news --search "ራሽያ"
+```
+ ![Made with VHS](https://vhs.charm.sh/vhs-3xJSIxwi4g5OS48lxdDFtP.gif)
+
+
+</details>
+
+<details>
+<summary>Export to file</summary>
+
+```bash
+# Export to file
+mereja --job --latest --export --path "jobs.json"
+
+# you can use the -e flag in any command to export to file i think :)
+```
+
+</details>
+
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+## License
+[MIT](https://choosealicense.com/licenses/mit/)
+
+
+
+
```

### Comparing `mereja-0.0.1/mereja.egg-info/SOURCES.txt` & `mereja-0.0.2/mereja.egg-info/SOURCES.txt`

 * *Files identical despite different names*

