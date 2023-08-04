# Comparing `tmp/powerjira-0.2.4.tar.gz` & `tmp/powerjira-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerjira-0.2.4.tar", max compression
+gzip compressed data, was "powerjira-0.2.5.tar", max compression
```

## Comparing `powerjira-0.2.4.tar` & `powerjira-0.2.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2022-09-15 05:28:05.416646 powerjira-0.2.4/LICENSE
--rw-r--r--   0        0        0     3245 2022-09-15 18:53:15.228276 powerjira-0.2.4/README.md
--rwxr-xr-x   0        0        0     2450 2023-08-04 21:22:24.231536 powerjira-0.2.4/powerjira.py
--rw-r--r--   0        0        0      661 2023-08-04 21:22:34.049018 powerjira-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     4493 2023-08-04 21:21:03.620758 powerjira-0.2.4/toolchain/commands.py
--rw-r--r--   0        0        0     1860 2023-08-04 20:12:56.534347 powerjira-0.2.4/toolchain/utils.py
--rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 powerjira-0.2.4/setup.py
--rw-r--r--   0        0        0     3963 1970-01-01 00:00:00.000000 powerjira-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-15 05:28:05.416646 powerjira-0.2.5/LICENSE
+-rw-r--r--   0        0        0     3245 2022-09-15 18:53:15.228276 powerjira-0.2.5/README.md
+-rwxr-xr-x   0        0        0     2450 2023-08-04 21:22:24.231536 powerjira-0.2.5/powerjira.py
+-rw-r--r--   0        0        0      661 2023-08-04 21:25:37.119203 powerjira-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     4508 2023-08-04 21:25:30.227267 powerjira-0.2.5/toolchain/commands.py
+-rw-r--r--   0        0        0     1860 2023-08-04 20:12:56.534347 powerjira-0.2.5/toolchain/utils.py
+-rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 powerjira-0.2.5/setup.py
+-rw-r--r--   0        0        0     3963 1970-01-01 00:00:00.000000 powerjira-0.2.5/PKG-INFO
```

### Comparing `powerjira-0.2.4/LICENSE` & `powerjira-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `powerjira-0.2.4/README.md` & `powerjira-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `powerjira-0.2.4/powerjira.py` & `powerjira-0.2.5/powerjira.py`

 * *Files identical despite different names*

### Comparing `powerjira-0.2.4/pyproject.toml` & `powerjira-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "powerjira"
-version = "0.2.4"
+version = "0.2.5"
 description = "A succinct, minimal local jira control plane that can live in your text editor. Interface with tickets fast!"
 authors = ["sleepyboy <anthonybenchyep@gmail.com>"]
 license = "GNU GPL"
 readme = "README.md"
 repository = "https://github.com/anthonybench/powerjira"
 keywords = ["jira", "poetry"]
 packages = [
```

### Comparing `powerjira-0.2.4/toolchain/commands.py` & `powerjira-0.2.5/toolchain/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     }
     ## publish
     try:
       if issueType.lower() == 'task':
         if epicKey:
           task_issue_blueprint['parent'] = {'key': epicKey}
         newIssue = jira.create_issue(fields=task_issue_blueprint)
-        print_issue(issue=newIssue, new=True, epic=False)
+        print_issue(issue=newIssue, domain=domain, new=True, epic=False)
         exit(0)
       elif issueType.lower() == 'epic':
         newIssue = jira.create_issue(fields=epic_issue_blueprint)
         print_issue(issue=newIssue, domain=domain, new=True, epic=True)
         exit(0)
       else:
         print(f'Error unsupported issue type.')
```

### Comparing `powerjira-0.2.4/toolchain/utils.py` & `powerjira-0.2.5/toolchain/utils.py`

 * *Files identical despite different names*

### Comparing `powerjira-0.2.4/setup.py` & `powerjira-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 modules = \
 ['powerjira', 'commands', 'utils']
 install_requires = \
 ['PyYAML>=6.0,<7.0', 'jira>=3.4.1,<4.0.0', 'typer>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'powerjira',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'A succinct, minimal local jira control plane that can live in your text editor. Interface with tickets fast!',
     'long_description': '# **PowerJira**\n*A succinct local jira control plane*\n\n<br />\n\n## **Welcome to PowerJira!**\nHate how visually noise and clunky the Jira web-app is? Ever wish you could just type the small subset of issue fields you actually care about into an editor and create/find tickets quickly?\n\nWelcome to the party! 🥳\n\n<br />\n\n### **Table of Contents** 📖\n<hr>\n\n  - [Welcome](#welcome-to-powerjira)\n  - [**Get Started**](#get-started-)\n  - [Usage](#usage-)\n  - [Technologies](#technologies-)\n  - [Contribute](#Contribute-)\n  - [Acknowledgements](#acknowledgements-)\n  - [License/Stats/Author](#license-stats-author-)\n\n<br />\n\n## **Get Started 🚀**\n<hr>\n\nTo get started, clone this repo and populate the config files per the readme.\n\nSpecifically, you need 4 files. These can be named whatever you wish by editing `main.py:59`. \\\nBelow are the requirements of the file with the default (suggested) file names:\n- `summary` - Text file for the issue summary\n- `description` - Text file for the issue description\n- `agent.yml` - Yaml file for user credentials\n- `config.yml` - Yaml file to configure issue creation\n\nThe text files simply contain the text you want in the ticket. \\\nAs for the yaml files, see the **Usage** section below.\n\nSet up your editor space the way you like it, and bam! You\'ve dramatically reduced your time spent in the jira web-app, and even possibly absolve the need for it completely!\n\n<br />\n\n## **Usage ⚙**\n<hr>\n\nWith your shell\'s working directory positioned where the 4 files are present (or if paths have been set accordingly):\n\n**Create ticket with config values**\n```sh\n./main.py [-r|--raw]\n```\n**Fetch info from existing ticket**\n```sh\n./main.py --fetch=<issue-key> [-r|--raw]\n```\n**Info**\n```sh\n./main.py [-h|--help]\n```\n\nThe "*raw*" option flag (`-r`, `--raw`) outputs a formatted dump of the raw api response.\n\nFor your own custom use:\n```python\nfrom powerjira import fetchIssue, createTicket\n```\n\nFor the configuration yaml\'s:\n**config.yml**\n```yaml\nproject:   <project-key>\npriority:  <priority>\n\nepicKey:   # Leave as empty for standalone task or epic\nissueType: <type>\n\nreporter:  <reporter-account-id>\nassignee:  <assignee-account-id>\n```\n**agent.yaml**\n```yaml\ndomain:   <host>\n\nuserName: <email>\ntoken:    <jira-access-token>\n```\n\n<br />\n\n## **Technologies 🧰**\n<hr>\n\n  - [PyYAML](https://pypi.org/project/PyYAML/)\n  - [python-jira](https://pypi.org/project/jira/)\n  - [Poetry](https://python-poetry.org/)\n\n<br />\n\n## **Contribute 🤝**\n<hr>\n\nFeel free to push PR\'s to help make this tool more extensible/flexible.\n\n<br />\n\n## **Acknowledgements 💙**\n<hr>\n\nThanks to Atlassian for making market-leading tools that kinda frustrate me.\n\n<br />\n\n## **License, Stats, Author 📜**\n<hr>\n\n<img align="right" alt="example image tag" src="https://i.imgur.com/jtNwEWu.png" width="200" />\n\n<!-- badge cluster -->\n\n![PyPI](https://img.shields.io/pypi/v/powerjira)\n![GitHub repo size](https://img.shields.io/github/repo-size/anthonybench/powerjira)\n\n<!-- / -->\nSee [License](https://www.gnu.org/licenses/gpl-3.0.txt) for the full license text.\n\nThis repository was authored by *Isaac Yep*. \\\n[PyPi Package](https://pypi.org/project/powerjira/#table-of-contents)\n\n[Back to Table of Contents](#table-of-contents-)',
     'author': 'sleepyboy',
     'author_email': 'anthonybenchyep@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/anthonybench/powerjira',
```

### Comparing `powerjira-0.2.4/PKG-INFO` & `powerjira-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerjira
-Version: 0.2.4
+Version: 0.2.5
 Summary: A succinct, minimal local jira control plane that can live in your text editor. Interface with tickets fast!
 Home-page: https://github.com/anthonybench/powerjira
 License: GNU GPL
 Keywords: jira,poetry
 Author: sleepyboy
 Author-email: anthonybenchyep@gmail.com
 Requires-Python: >=3.10,<4.0
```

