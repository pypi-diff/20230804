# Comparing `tmp/powerjira-0.1.7.tar.gz` & `tmp/powerjira-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerjira-0.1.7.tar", max compression
+gzip compressed data, was "powerjira-0.1.9.tar", max compression
```

## Comparing `powerjira-0.1.7.tar` & `powerjira-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     3105 2022-09-15 18:53:54.378130 powerjira-0.1.7/README.md
--rw-r--r--   0        0        0     7221 2022-09-15 16:54:10.976448 powerjira-0.1.7/powerjira.py
--rw-r--r--   0        0        0      519 2022-09-15 18:54:03.133624 powerjira-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3930 1970-01-01 00:00:00.000000 powerjira-0.1.7/setup.py
--rw-r--r--   0        0        0     3784 1970-01-01 00:00:00.000000 powerjira-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-15 05:28:05.416646 powerjira-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3245 2022-09-15 18:53:15.228276 powerjira-0.1.9/README.md
+-rwxr-xr-x   0        0        0     2034 2023-08-04 20:04:52.626292 powerjira-0.1.9/powerjira.py
+-rw-r--r--   0        0        0      661 2023-08-04 20:35:54.766291 powerjira-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3709 2023-08-04 20:13:31.957404 powerjira-0.1.9/toolchain/commands.py
+-rw-r--r--   0        0        0     1860 2023-08-04 20:12:56.534347 powerjira-0.1.9/toolchain/utils.py
+-rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 powerjira-0.1.9/setup.py
+-rw-r--r--   0        0        0     3963 1970-01-01 00:00:00.000000 powerjira-0.1.9/PKG-INFO
```

### Comparing `powerjira-0.1.7/README.md` & `powerjira-0.1.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 Welcome to the party! 🥳
 
 <br />
 
 ### **Table of Contents** 📖
 <hr>
 
-  - **Get Started**
-  - Usage
-  - Technologies
-  - Contribute
-  - Acknowledgements
-  - License/Stats/Author
+  - [Welcome](#welcome-to-powerjira)
+  - [**Get Started**](#get-started-)
+  - [Usage](#usage-)
+  - [Technologies](#technologies-)
+  - [Contribute](#Contribute-)
+  - [Acknowledgements](#acknowledgements-)
+  - [License/Stats/Author](#license-stats-author-)
 
 <br />
 
 ## **Get Started 🚀**
 <hr>
 
-To get started, clone the [interface repository](https://github.com/anthonybench/powerjira) and populate the config files per the readme.
+To get started, clone this repo and populate the config files per the readme.
 
 Specifically, you need 4 files. These can be named whatever you wish by editing `main.py:59`. \
 Below are the requirements of the file with the default (suggested) file names:
 - `summary` - Text file for the issue summary
 - `description` - Text file for the issue description
 - `agent.yml` - Yaml file for user credentials
 - `config.yml` - Yaml file to configure issue creation
@@ -96,15 +97,15 @@
   - [Poetry](https://python-poetry.org/)
 
 <br />
 
 ## **Contribute 🤝**
 <hr>
 
-Feel free to push PR's to help make this tool more extensible/flexible over at the [GitHub repo](https://github.com/anthonybench/powerjira).
+Feel free to push PR's to help make this tool more extensible/flexible.
 
 <br />
 
 ## **Acknowledgements 💙**
 <hr>
 
 Thanks to Atlassian for making market-leading tools that kinda frustrate me.
@@ -120,8 +121,11 @@
 
 ![PyPI](https://img.shields.io/pypi/v/powerjira)
 ![GitHub repo size](https://img.shields.io/github/repo-size/anthonybench/powerjira)
 
 <!-- / -->
 See [License](https://www.gnu.org/licenses/gpl-3.0.txt) for the full license text.
 
-This repository was authored by *Isaac Yep*.
+This repository was authored by *Isaac Yep*. \
+[PyPi Package](https://pypi.org/project/powerjira/#table-of-contents)
+
+[Back to Table of Contents](#table-of-contents-)
```

### Comparing `powerjira-0.1.7/pyproject.toml` & `powerjira-0.1.9/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 [tool.poetry]
 name = "powerjira"
-version = "0.1.7"
+version = "0.1.9"
 description = "A succinct, minimal local jira control plane that can live in your text editor. Interface with tickets fast!"
 authors = ["sleepyboy <anthonybenchyep@gmail.com>"]
 license = "GNU GPL"
 readme = "README.md"
 repository = "https://github.com/anthonybench/powerjira"
 keywords = ["jira", "poetry"]
+packages = [
+  { include = "powerjira.py" },
+  { include = "toolchain/commands.py" },
+  { include = "toolchain/utils.py" },
+]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 PyYAML = "^6.0"
 jira = "^3.4.1"
-
+typer = "^0.9.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `powerjira-0.1.7/setup.py` & `powerjira-0.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
-['powerjira']
+['powerjira', 'commands', 'utils']
 install_requires = \
-['PyYAML>=6.0,<7.0', 'jira>=3.4.1,<4.0.0']
+['PyYAML>=6.0,<7.0', 'jira>=3.4.1,<4.0.0', 'typer>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'powerjira',
-    'version': '0.1.7',
+    'version': '0.1.9',
     'description': 'A succinct, minimal local jira control plane that can live in your text editor. Interface with tickets fast!',
-    'long_description': '# **PowerJira**\n*A succinct local jira control plane*\n\n<br />\n\n## **Welcome to PowerJira!**\nHate how visually noise and clunky the Jira web-app is? Ever wish you could just type the small subset of issue fields you actually care about into an editor and create/find tickets quickly?\n\nWelcome to the party! 🥳\n\n<br />\n\n### **Table of Contents** 📖\n<hr>\n\n  - **Get Started**\n  - Usage\n  - Technologies\n  - Contribute\n  - Acknowledgements\n  - License/Stats/Author\n\n<br />\n\n## **Get Started 🚀**\n<hr>\n\nTo get started, clone the [interface repository](https://github.com/anthonybench/powerjira) and populate the config files per the readme.\n\nSpecifically, you need 4 files. These can be named whatever you wish by editing `main.py:59`. \\\nBelow are the requirements of the file with the default (suggested) file names:\n- `summary` - Text file for the issue summary\n- `description` - Text file for the issue description\n- `agent.yml` - Yaml file for user credentials\n- `config.yml` - Yaml file to configure issue creation\n\nThe text files simply contain the text you want in the ticket. \\\nAs for the yaml files, see the **Usage** section below.\n\nSet up your editor space the way you like it, and bam! You\'ve dramatically reduced your time spent in the jira web-app, and even possibly absolve the need for it completely!\n\n<br />\n\n## **Usage ⚙**\n<hr>\n\nWith your shell\'s working directory positioned where the 4 files are present (or if paths have been set accordingly):\n\n**Create ticket with config values**\n```sh\n./main.py [-r|--raw]\n```\n**Fetch info from existing ticket**\n```sh\n./main.py --fetch=<issue-key> [-r|--raw]\n```\n**Info**\n```sh\n./main.py [-h|--help]\n```\n\nThe "*raw*" option flag (`-r`, `--raw`) outputs a formatted dump of the raw api response.\n\nFor your own custom use:\n```python\nfrom powerjira import fetchIssue, createTicket\n```\n\nFor the configuration yaml\'s:\n**config.yml**\n```yaml\nproject:   <project-key>\npriority:  <priority>\n\nepicKey:   # Leave as empty for standalone task or epic\nissueType: <type>\n\nreporter:  <reporter-account-id>\nassignee:  <assignee-account-id>\n```\n**agent.yaml**\n```yaml\ndomain:   <host>\n\nuserName: <email>\ntoken:    <jira-access-token>\n```\n\n<br />\n\n## **Technologies 🧰**\n<hr>\n\n  - [PyYAML](https://pypi.org/project/PyYAML/)\n  - [python-jira](https://pypi.org/project/jira/)\n  - [Poetry](https://python-poetry.org/)\n\n<br />\n\n## **Contribute 🤝**\n<hr>\n\nFeel free to push PR\'s to help make this tool more extensible/flexible over at the [GitHub repo](https://github.com/anthonybench/powerjira).\n\n<br />\n\n## **Acknowledgements 💙**\n<hr>\n\nThanks to Atlassian for making market-leading tools that kinda frustrate me.\n\n<br />\n\n## **License, Stats, Author 📜**\n<hr>\n\n<img align="right" alt="example image tag" src="https://i.imgur.com/jtNwEWu.png" width="200" />\n\n<!-- badge cluster -->\n\n![PyPI](https://img.shields.io/pypi/v/powerjira)\n![GitHub repo size](https://img.shields.io/github/repo-size/anthonybench/powerjira)\n\n<!-- / -->\nSee [License](https://www.gnu.org/licenses/gpl-3.0.txt) for the full license text.\n\nThis repository was authored by *Isaac Yep*.',
+    'long_description': '# **PowerJira**\n*A succinct local jira control plane*\n\n<br />\n\n## **Welcome to PowerJira!**\nHate how visually noise and clunky the Jira web-app is? Ever wish you could just type the small subset of issue fields you actually care about into an editor and create/find tickets quickly?\n\nWelcome to the party! 🥳\n\n<br />\n\n### **Table of Contents** 📖\n<hr>\n\n  - [Welcome](#welcome-to-powerjira)\n  - [**Get Started**](#get-started-)\n  - [Usage](#usage-)\n  - [Technologies](#technologies-)\n  - [Contribute](#Contribute-)\n  - [Acknowledgements](#acknowledgements-)\n  - [License/Stats/Author](#license-stats-author-)\n\n<br />\n\n## **Get Started 🚀**\n<hr>\n\nTo get started, clone this repo and populate the config files per the readme.\n\nSpecifically, you need 4 files. These can be named whatever you wish by editing `main.py:59`. \\\nBelow are the requirements of the file with the default (suggested) file names:\n- `summary` - Text file for the issue summary\n- `description` - Text file for the issue description\n- `agent.yml` - Yaml file for user credentials\n- `config.yml` - Yaml file to configure issue creation\n\nThe text files simply contain the text you want in the ticket. \\\nAs for the yaml files, see the **Usage** section below.\n\nSet up your editor space the way you like it, and bam! You\'ve dramatically reduced your time spent in the jira web-app, and even possibly absolve the need for it completely!\n\n<br />\n\n## **Usage ⚙**\n<hr>\n\nWith your shell\'s working directory positioned where the 4 files are present (or if paths have been set accordingly):\n\n**Create ticket with config values**\n```sh\n./main.py [-r|--raw]\n```\n**Fetch info from existing ticket**\n```sh\n./main.py --fetch=<issue-key> [-r|--raw]\n```\n**Info**\n```sh\n./main.py [-h|--help]\n```\n\nThe "*raw*" option flag (`-r`, `--raw`) outputs a formatted dump of the raw api response.\n\nFor your own custom use:\n```python\nfrom powerjira import fetchIssue, createTicket\n```\n\nFor the configuration yaml\'s:\n**config.yml**\n```yaml\nproject:   <project-key>\npriority:  <priority>\n\nepicKey:   # Leave as empty for standalone task or epic\nissueType: <type>\n\nreporter:  <reporter-account-id>\nassignee:  <assignee-account-id>\n```\n**agent.yaml**\n```yaml\ndomain:   <host>\n\nuserName: <email>\ntoken:    <jira-access-token>\n```\n\n<br />\n\n## **Technologies 🧰**\n<hr>\n\n  - [PyYAML](https://pypi.org/project/PyYAML/)\n  - [python-jira](https://pypi.org/project/jira/)\n  - [Poetry](https://python-poetry.org/)\n\n<br />\n\n## **Contribute 🤝**\n<hr>\n\nFeel free to push PR\'s to help make this tool more extensible/flexible.\n\n<br />\n\n## **Acknowledgements 💙**\n<hr>\n\nThanks to Atlassian for making market-leading tools that kinda frustrate me.\n\n<br />\n\n## **License, Stats, Author 📜**\n<hr>\n\n<img align="right" alt="example image tag" src="https://i.imgur.com/jtNwEWu.png" width="200" />\n\n<!-- badge cluster -->\n\n![PyPI](https://img.shields.io/pypi/v/powerjira)\n![GitHub repo size](https://img.shields.io/github/repo-size/anthonybench/powerjira)\n\n<!-- / -->\nSee [License](https://www.gnu.org/licenses/gpl-3.0.txt) for the full license text.\n\nThis repository was authored by *Isaac Yep*. \\\n[PyPi Package](https://pypi.org/project/powerjira/#table-of-contents)\n\n[Back to Table of Contents](#table-of-contents-)',
     'author': 'sleepyboy',
     'author_email': 'anthonybenchyep@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/anthonybench/powerjira',
     'py_modules': modules,
     'install_requires': install_requires,
```

### Comparing `powerjira-0.1.7/PKG-INFO` & `powerjira-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: powerjira
-Version: 0.1.7
+Version: 0.1.9
 Summary: A succinct, minimal local jira control plane that can live in your text editor. Interface with tickets fast!
 Home-page: https://github.com/anthonybench/powerjira
 License: GNU GPL
 Keywords: jira,poetry
 Author: sleepyboy
 Author-email: anthonybenchyep@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: jira (>=3.4.1,<4.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/anthonybench/powerjira
 Description-Content-Type: text/markdown
 
 # **PowerJira**
 *A succinct local jira control plane*
 
 <br />
@@ -27,27 +28,28 @@
 Welcome to the party! 🥳
 
 <br />
 
 ### **Table of Contents** 📖
 <hr>
 
-  - **Get Started**
-  - Usage
-  - Technologies
-  - Contribute
-  - Acknowledgements
-  - License/Stats/Author
+  - [Welcome](#welcome-to-powerjira)
+  - [**Get Started**](#get-started-)
+  - [Usage](#usage-)
+  - [Technologies](#technologies-)
+  - [Contribute](#Contribute-)
+  - [Acknowledgements](#acknowledgements-)
+  - [License/Stats/Author](#license-stats-author-)
 
 <br />
 
 ## **Get Started 🚀**
 <hr>
 
-To get started, clone the [interface repository](https://github.com/anthonybench/powerjira) and populate the config files per the readme.
+To get started, clone this repo and populate the config files per the readme.
 
 Specifically, you need 4 files. These can be named whatever you wish by editing `main.py:59`. \
 Below are the requirements of the file with the default (suggested) file names:
 - `summary` - Text file for the issue summary
 - `description` - Text file for the issue description
 - `agent.yml` - Yaml file for user credentials
 - `config.yml` - Yaml file to configure issue creation
@@ -114,15 +116,15 @@
   - [Poetry](https://python-poetry.org/)
 
 <br />
 
 ## **Contribute 🤝**
 <hr>
 
-Feel free to push PR's to help make this tool more extensible/flexible over at the [GitHub repo](https://github.com/anthonybench/powerjira).
+Feel free to push PR's to help make this tool more extensible/flexible.
 
 <br />
 
 ## **Acknowledgements 💙**
 <hr>
 
 Thanks to Atlassian for making market-leading tools that kinda frustrate me.
@@ -138,8 +140,11 @@
 
 ![PyPI](https://img.shields.io/pypi/v/powerjira)
 ![GitHub repo size](https://img.shields.io/github/repo-size/anthonybench/powerjira)
 
 <!-- / -->
 See [License](https://www.gnu.org/licenses/gpl-3.0.txt) for the full license text.
 
-This repository was authored by *Isaac Yep*.
+This repository was authored by *Isaac Yep*. \
+[PyPi Package](https://pypi.org/project/powerjira/#table-of-contents)
+
+[Back to Table of Contents](#table-of-contents-)
```

