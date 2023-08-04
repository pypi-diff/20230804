# Comparing `tmp/gitea_github_sync-0.1.1.tar.gz` & `tmp/gitea_github_sync-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitea_github_sync-0.1.1.tar", max compression
+gzip compressed data, was "gitea_github_sync-0.1.2.tar", max compression
```

## Comparing `gitea_github_sync-0.1.1.tar` & `gitea_github_sync-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1071 2023-01-05 16:41:32.569152 gitea_github_sync-0.1.1/LICENSE
--rw-r--r--   0        0        0     2521 2023-01-05 16:41:32.569152 gitea_github_sync-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-01-05 16:41:32.573152 gitea_github_sync-0.1.1/gitea_github_sync/__init__.py
--rw-r--r--   0        0        0       29 2023-01-05 16:41:32.573152 gitea_github_sync-0.1.1/gitea_github_sync/__main__.py
--rw-r--r--   0        0        0     2693 2023-01-05 16:41:32.573152 gitea_github_sync-0.1.1/gitea_github_sync/cli.py
--rw-r--r--   0        0        0      637 2023-01-05 16:41:32.573152 gitea_github_sync-0.1.1/gitea_github_sync/config.py
--rw-r--r--   0        0        0     2298 2023-01-05 16:41:32.573152 gitea_github_sync-0.1.1/gitea_github_sync/gitea.py
--rw-r--r--   0        0        0      619 2023-01-05 16:41:32.573152 gitea_github_sync-0.1.1/gitea_github_sync/github.py
--rw-r--r--   0        0        0      358 2023-01-05 16:41:32.573152 gitea_github_sync-0.1.1/gitea_github_sync/migration.py
--rw-r--r--   0        0        0      705 2023-01-05 16:41:32.573152 gitea_github_sync-0.1.1/gitea_github_sync/repository.py
--rw-r--r--   0        0        0     1512 2023-01-05 16:41:32.573152 gitea_github_sync-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3558 1970-01-01 00:00:00.000000 gitea_github_sync-0.1.1/setup.py
--rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 gitea_github_sync-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-04 20:16:30.917635 gitea_github_sync-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2997 2023-08-04 20:16:30.921635 gitea_github_sync-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-08-04 20:16:30.921635 gitea_github_sync-0.1.2/gitea_github_sync/__init__.py
+-rw-r--r--   0        0        0       29 2023-08-04 20:16:30.921635 gitea_github_sync-0.1.2/gitea_github_sync/__main__.py
+-rw-r--r--   0        0        0     2693 2023-08-04 20:16:30.921635 gitea_github_sync-0.1.2/gitea_github_sync/cli.py
+-rw-r--r--   0        0        0      636 2023-08-04 20:16:30.921635 gitea_github_sync-0.1.2/gitea_github_sync/config.py
+-rw-r--r--   0        0        0     2297 2023-08-04 20:16:30.921635 gitea_github_sync-0.1.2/gitea_github_sync/gitea.py
+-rw-r--r--   0        0        0      619 2023-08-04 20:16:30.921635 gitea_github_sync-0.1.2/gitea_github_sync/github.py
+-rw-r--r--   0        0        0      358 2023-08-04 20:16:30.921635 gitea_github_sync-0.1.2/gitea_github_sync/migration.py
+-rw-r--r--   0        0        0      705 2023-08-04 20:16:30.921635 gitea_github_sync-0.1.2/gitea_github_sync/repository.py
+-rw-r--r--   0        0        0     1540 2023-08-04 20:16:30.921635 gitea_github_sync-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4235 1970-01-01 00:00:00.000000 gitea_github_sync-0.1.2/PKG-INFO
```

### Comparing `gitea_github_sync-0.1.1/LICENSE` & `gitea_github_sync-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gitea_github_sync-0.1.1/README.md` & `gitea_github_sync-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/gitea-github-sync/0.1.0)](https://pypi.org/project/gitea-github-sync/) [![PyPI version](https://badge.fury.io/py/gitea-github-sync.svg)](https://badge.fury.io/py/gitea-github-sync)
+
+[![codecov](https://img.shields.io/codecov/c/github/Muscaw/gitea-github-sync?label=codecov&logo=codecov)](https://codecov.io/gh/Muscaw/gitea-github-sync) ![PyPI - Downloads](https://img.shields.io/pypi/dm/gitea-github-sync)
+
 # gitea-github-sync
 
 gitea-github-sync provides a simple CLI to sync Github repositories to your Gitea instance.
 
 ## Installation
 
 ```
```

### Comparing `gitea_github_sync-0.1.1/gitea_github_sync/cli.py` & `gitea_github_sync-0.1.2/gitea_github_sync/cli.py`

 * *Files identical despite different names*

### Comparing `gitea_github_sync-0.1.1/gitea_github_sync/config.py` & `gitea_github_sync-0.1.2/gitea_github_sync/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 
 def config_file_location() -> Path:
     return Path.home() / ".config" / "gitea-github-sync" / "config.yml"
 
 
 def load_config(config_location: Path = config_file_location()) -> Config:
-
     return Config(
         **YamlLoader(
             path=config_location,
             matcher=StrictMatcher,
             validator=PydanticValidator,
             schema=Config,
         ).load()
```

### Comparing `gitea_github_sync-0.1.1/gitea_github_sync/gitea.py` & `gitea_github_sync-0.1.2/gitea_github_sync/gitea.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
             data = result.json()
             output.extend(data)
 
             url = result.links["next"]["url"] if "next" in result.links else None
         return output
 
     def get_repos(self) -> List[Repository]:
-
         repos = self._get_all_pages("/user/repos")
         return [
             Repository(
                 repo["full_name"],
                 visibility=Visibility.PRIVATE if repo["private"] else Visibility.PUBLIC,
             )
             for repo in repos
```

### Comparing `gitea_github_sync-0.1.1/gitea_github_sync/github.py` & `gitea_github_sync-0.1.2/gitea_github_sync/github.py`

 * *Files identical despite different names*

### Comparing `gitea_github_sync-0.1.1/gitea_github_sync/repository.py` & `gitea_github_sync-0.1.2/gitea_github_sync/repository.py`

 * *Files identical despite different names*

### Comparing `gitea_github_sync-0.1.1/pyproject.toml` & `gitea_github_sync-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 profile = "black"
 
 [tool.black]
 line-length = 100
 
 [tool.poetry]
 name = "gitea-github-sync"
-version = "0.1.1"
+version = "0.1.2"
 homepage = "https://github.com/Muscaw/gitea-github-sync"
 description = "Syncs your gitea instance with your Github account"
 authors = ["Kevin Grandjean <Muscaw@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -32,29 +32,29 @@
 [tool.poetry.scripts]
 gitea-github-sync = "gitea_github_sync.cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 pygithub = "^1.57"
 click = "^8.1.3"
-piny = "^0.6.0"
-pydantic = "^1.10.4"
+piny = ">=0.6,<1.1"
+pydantic = ">=1.10.4,<3.0.0"
 rich = "^13.0.0"
 requests = "^2.28.1"
 
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
-black = "^22.12.0"
+black = ">=22.12,<24.0"
 flake8 = "^6.0.0"
 isort = "^5.11.4"
-mypy = "^0.991"
+mypy = ">=0.991,<1.5"
 tox = "^4.1.1"
 pytest-cov = "^4.0.0"
-responses = "^0.22.0"
+responses = ">=0.22,<0.24"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gitea_github_sync-0.1.1/setup.py` & `gitea_github_sync-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,106 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: gitea-github-sync
+Version: 0.1.2
+Summary: Syncs your gitea instance with your Github account
+Home-page: https://github.com/Muscaw/gitea-github-sync
+License: MIT
+Author: Kevin Grandjean
+Author-email: Muscaw@users.noreply.github.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Typing :: Typed
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: piny (>=0.6,<1.1)
+Requires-Dist: pydantic (>=1.10.4,<3.0.0)
+Requires-Dist: pygithub (>=1.57,<2.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: rich (>=13.0.0,<14.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['gitea_github_sync']
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/gitea-github-sync/0.1.0)](https://pypi.org/project/gitea-github-sync/) [![PyPI version](https://badge.fury.io/py/gitea-github-sync.svg)](https://badge.fury.io/py/gitea-github-sync)
 
-package_data = \
-{'': ['*']}
+[![codecov](https://img.shields.io/codecov/c/github/Muscaw/gitea-github-sync?label=codecov&logo=codecov)](https://codecov.io/gh/Muscaw/gitea-github-sync) ![PyPI - Downloads](https://img.shields.io/pypi/dm/gitea-github-sync)
 
-install_requires = \
-['click>=8.1.3,<9.0.0',
- 'piny>=0.6.0,<0.7.0',
- 'pydantic>=1.10.4,<2.0.0',
- 'pygithub>=1.57,<2.0',
- 'requests>=2.28.1,<3.0.0',
- 'rich>=13.0.0,<14.0.0']
-
-entry_points = \
-{'console_scripts': ['gitea-github-sync = gitea_github_sync.cli:cli']}
-
-setup_kwargs = {
-    'name': 'gitea-github-sync',
-    'version': '0.1.1',
-    'description': 'Syncs your gitea instance with your Github account',
-    'long_description': '# gitea-github-sync\n\ngitea-github-sync provides a simple CLI to sync Github repositories to your Gitea instance.\n\n## Installation\n\n```\npip install gitea-github-sync\n```\n\nIf you are interested in using a pre-packaged docker image, please look at the [Docker Readme](docs/docker/README.md)\n\n## Setup\nCreate a file in `$HOME/.config/gitea-github-sync/config.yml` with the following template and fill up the missing values:\n\n```yaml\ngitea_api_url: https://<your-gitea-instance>/api/v1\ngitea_token: <your-gitea-token>\ngithub_token: <your-github-token>\n```\n\n### Creating a Gitea token\nGo to https://\\<your-local-gitea-instance\\>/user/settings/applications and generate a new token.\n\n### Creating a Github token\n\nGo to https://github.com/settings/tokens/new and create a token with the following values set:\n- Note: this is a note to help you understand how the token is used.\n- Expiration: No expiration\n- repo: Select all of repo\n\n![Screenshot of token configuration](docs/readme/github_token_permission.png)\n\n#### Github token limitation\nGithub allows you to create _Personal access tokens_. These tokens now exist in two different flavors:\n- Fine-grained tokens\n- Classic tokens\n\nBoth work with gitea-github-sync, but given that Gitea does not allow the modification of the access token through the API, a **non-expiring** token must be used which limits the usage to Classic tokens.\n\n## Usage\n\n`gitea-github-sync --help` Shows the help\n\n`gitea-github-sync list-all-gitea-repositories` Lists all available Gitea repositories in your account\n\n`gitea-github-sync list-all-github-repositories` Lists all available Github repositories in your account\n\n`gitea-github-sync migrate-repo FULL_REPO_NAME` Migrates one repo from Github to Gitea\n\n`gitea-github-sync sync` Migrates all repos not present in Gitea from Github\n\n## Automate gitea-github-sync execution\n\nThere are multiple ways to automate the execution of gitea-github-sync. One of them is using cron:\n\nFirst, execute `crontab -e` to open the cron configuration file in edit mode.\n\nThen add the following line:\n```\n0 12 * * * gitea-github-sync sync\n```\n\nThis will execute the sync operation every day at twelve.\n\n## Limitations\n\nWhen using the migration feature of Gitea, a Github token must be passed for Gitea to continuously pull the new changes from Github.\n\nThe token used by gitea-github-sync to list repositories is the same that is used by Gitea for continuous monitoring. Updating the value of this token is unfortunately not possible through the API as of now. \n',
-    'author': 'Kevin Grandjean',
-    'author_email': 'Muscaw@users.noreply.github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Muscaw/gitea-github-sync',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8.1,<4.0.0',
-}
+# gitea-github-sync
 
+gitea-github-sync provides a simple CLI to sync Github repositories to your Gitea instance.
+
+## Installation
+
+```
+pip install gitea-github-sync
+```
+
+If you are interested in using a pre-packaged docker image, please look at the [Docker Readme](docs/docker/README.md)
+
+## Setup
+Create a file in `$HOME/.config/gitea-github-sync/config.yml` with the following template and fill up the missing values:
+
+```yaml
+gitea_api_url: https://<your-gitea-instance>/api/v1
+gitea_token: <your-gitea-token>
+github_token: <your-github-token>
+```
+
+### Creating a Gitea token
+Go to https://\<your-local-gitea-instance\>/user/settings/applications and generate a new token.
+
+### Creating a Github token
+
+Go to https://github.com/settings/tokens/new and create a token with the following values set:
+- Note: this is a note to help you understand how the token is used.
+- Expiration: No expiration
+- repo: Select all of repo
+
+![Screenshot of token configuration](docs/readme/github_token_permission.png)
+
+#### Github token limitation
+Github allows you to create _Personal access tokens_. These tokens now exist in two different flavors:
+- Fine-grained tokens
+- Classic tokens
+
+Both work with gitea-github-sync, but given that Gitea does not allow the modification of the access token through the API, a **non-expiring** token must be used which limits the usage to Classic tokens.
+
+## Usage
+
+`gitea-github-sync --help` Shows the help
+
+`gitea-github-sync list-all-gitea-repositories` Lists all available Gitea repositories in your account
+
+`gitea-github-sync list-all-github-repositories` Lists all available Github repositories in your account
+
+`gitea-github-sync migrate-repo FULL_REPO_NAME` Migrates one repo from Github to Gitea
+
+`gitea-github-sync sync` Migrates all repos not present in Gitea from Github
+
+## Automate gitea-github-sync execution
+
+There are multiple ways to automate the execution of gitea-github-sync. One of them is using cron:
+
+First, execute `crontab -e` to open the cron configuration file in edit mode.
+
+Then add the following line:
+```
+0 12 * * * gitea-github-sync sync
+```
+
+This will execute the sync operation every day at twelve.
+
+## Limitations
+
+When using the migration feature of Gitea, a Github token must be passed for Gitea to continuously pull the new changes from Github.
+
+The token used by gitea-github-sync to list repositories is the same that is used by Gitea for continuous monitoring. Updating the value of this token is unfortunately not possible through the API as of now. 
 
-setup(**setup_kwargs)
```

