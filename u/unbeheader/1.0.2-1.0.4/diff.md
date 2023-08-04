# Comparing `tmp/unbeheader-1.0.2.tar.gz` & `tmp/unbeheader-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbeheader-1.0.2.tar", max compression
+gzip compressed data, was "unbeheader-1.0.4.tar", max compression
```

## Comparing `unbeheader-1.0.2.tar` & `unbeheader-1.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1139 2023-08-04 01:05:09.728586 unbeheader-1.0.2/LICENSE
--rw-r--r--   0        0        0     6427 2023-08-04 01:05:09.728586 unbeheader-1.0.2/README.md
--rw-r--r--   0        0        0     1009 2023-08-04 01:05:09.728586 unbeheader-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1848 2023-08-04 01:05:09.728586 unbeheader-1.0.2/unbeheader/__init__.py
--rw-r--r--   0        0        0     3718 2023-08-04 01:05:09.728586 unbeheader-1.0.2/unbeheader/cli.py
--rw-r--r--   0        0        0     2112 2023-08-04 01:05:09.728586 unbeheader-1.0.2/unbeheader/config.py
--rw-r--r--   0        0        0     2802 2023-08-04 01:05:09.728586 unbeheader-1.0.2/unbeheader/headers.py
--rw-r--r--   0        0        0     1747 2023-08-04 01:05:09.728586 unbeheader-1.0.2/unbeheader/util.py
--rw-r--r--   0        0        0     7434 1970-01-01 00:00:00.000000 unbeheader-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1139 2023-08-04 01:30:37.677971 unbeheader-1.0.4/LICENSE
+-rw-r--r--   0        0        0     6408 2023-08-04 01:30:37.677971 unbeheader-1.0.4/README.md
+-rw-r--r--   0        0        0     1007 2023-08-04 01:30:37.677971 unbeheader-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1848 2023-08-04 01:30:37.677971 unbeheader-1.0.4/unbeheader/__init__.py
+-rw-r--r--   0        0        0     3718 2023-08-04 01:30:37.677971 unbeheader-1.0.4/unbeheader/cli.py
+-rw-r--r--   0        0        0     2112 2023-08-04 01:30:37.677971 unbeheader-1.0.4/unbeheader/config.py
+-rw-r--r--   0        0        0     2802 2023-08-04 01:30:37.677971 unbeheader-1.0.4/unbeheader/headers.py
+-rw-r--r--   0        0        0     1747 2023-08-04 01:30:37.677971 unbeheader-1.0.4/unbeheader/util.py
+-rw-r--r--   0        0        0     7415 1970-01-01 00:00:00.000000 unbeheader-1.0.4/PKG-INFO
```

### Comparing `unbeheader-1.0.2/LICENSE` & `unbeheader-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unbeheader-1.0.2/README.md` & `unbeheader-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,33 +38,33 @@
 
 ### Usage
 
 It's possible to run Unbeheader in two modes: `fix` and `check`. The `fix` mode will update all files in the project with the correct header. The `check` mode will check that all files in the project have the correct header and exit with a non-zero status code if any file is missing or has an incorrect header.
 
 > **NOTE:** Neither `fix` or `check` modes will work unless Unbeheader can find a `.header.yaml` configuration file. Read more on the [Configuration](#configuration) section.
 
-To run Unbeheader in `fix` mode simply run the `unbeheader` command:
+To run Unbeheader in `fix` mode simply run the `unbehead` command:
 
 ```sh
-unbeheader                            # Update all the files in the Git repository
-unbeheader --path .                   # Update all the files under the current directory
-unbeheader --path /path/to/directory  # Update all the files under a directory
-unbeheader --path /path/to/file.py    # Update a single file
+unbehead                            # Update all the files in the Git repository
+unbehead --path .                   # Update all the files under the current directory
+unbehead --path /path/to/directory  # Update all the files under a directory
+unbehead --path /path/to/file.py    # Update a single file
 ```
 
 By default, Unbeheader will pass the current year to generate the `{dates}` placeholder in the header template. To pass a different year, use the `--year` flag:
 
 ```sh
-unbeheader --year 1947
+unbehead --year 1947
 ```
 
 To run Unbeheader in `check` mode, use the `--ci` flag:
 
 ```sh
-unbehader --ci
+unbehead --ci
 ```
 
 ## Configuration
 
 Unbeheader reads its configuration from `.header.yaml` files placed in the file tree of the project. It is possible to override configuration values by placing `.header.yaml` files in subdirectories. This is useful when different headers are needed for different parts of the project. It is also possible to exclude a directory by placing an empty `.no-header` file in it.
 
 Here is an example of a project structure with various `.header.yaml` and `.no-header` files:
@@ -95,15 +95,15 @@
 
 Setting value keys:
 - `root`: When set to `true`, it will stop Unbeheader from looking for `.header.yaml` files in parent directories. It defaults to `false`.
 - `substring`: The substring that Unbeheader will look for to determine if a file has a header or not. If the substring is not found, Unbeheader will assume that the file has no header. It defaults to `This file is part of`.
 
 Template value keys:
 - `owner`: The owner of the project, used to generate the `{owner}` placeholder. This key is required.
-- `start_year`: The start year of the header, used to generate the `{dates}` placeholder. It defaults to the year passed to the `unbeheader` command.
+- `start_year`: The start year of the header, used to generate the `{dates}` placeholder. It defaults to the year passed to the `unbehead` command.
 
 Finally, the `template` key is a multi-line string that will be used to generate the header template. The template accepts the interpolation of certain placeholders. These are:
 
 - `{comment_start}`: The comment start string for the file type (e.g. `#` for Python files).
 - `{comment_middle}`: The comment middle string for the file type (e.g. ` *` for CSS files).
 - `{comment_end}`: The comment end string for the file type (e.g. ` */` for CSS files).
 - `{dates}`: The start and end years of the header (e.g. `1904 - 1947`).
@@ -133,25 +133,25 @@
 
 You may now create the virtualenv and install the project with its dependencies in it with `poetry`:
 
 ```sh
 poetry install
 ```
 
-Once installed, you can invoke the `unbeheader` command with:
+Once installed, you can invoke the `unbehead` command with:
 
 ```sh
 poetry run -- unbeheader
 ```
 
 For convenience, you may want to spawn a shell within the virtualenv with:
 
 ```sh
 poetry shell
-unbeheader
+unbehead
 ```
 
 ### Contributing
 
 This project uses GitHub Actions to run the tests and linter on every pull request to the `master` and `devel` branches. You are still encouraged to run the tests and linter locally before pushing your changes.
 
 Tests can be run with:
```

### Comparing `unbeheader-1.0.2/pyproject.toml` & `unbeheader-1.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [virtualenvs]
 create = true
 in-project = true
 
 [tool.poetry]
 name = "unbeheader"
-version = "1.0.2"
+version = "1.0.4"
 description = "Never fail to maintain your file headers"
 repository = "https://github.com/unconventional/unbeheader"
 readme = "README.md"
 license = "MIT"
 authors = [
   "Adrian Moennich <adrian.moennich@cern.ch>",
   "Alejandro Avilés <ome@unconventional.dev>"
@@ -21,15 +21,15 @@
     "Development Status :: 5 - Production/Stable",
     "Topic :: Software Development",
     "Topic :: Software Development :: Quality Assurance",
     "Topic :: Software Development :: Testing",
 ]
 
 [tool.poetry.scripts]
-unbeheader = "unbeheader.cli:main"
+unbehead = "unbeheader.cli:main"
 
 [tool.poetry.dependencies]
 python = ">=3.9.0"
 colorclass = ">=2.2.2"
 pyyaml = ">=6.0.1"
 click = ">=8.1.6"
```

### Comparing `unbeheader-1.0.2/unbeheader/__init__.py` & `unbeheader-1.0.4/unbeheader/__init__.py`

 * *Files identical despite different names*

### Comparing `unbeheader-1.0.2/unbeheader/cli.py` & `unbeheader-1.0.4/unbeheader/cli.py`

 * *Files identical despite different names*

### Comparing `unbeheader-1.0.2/unbeheader/config.py` & `unbeheader-1.0.4/unbeheader/config.py`

 * *Files identical despite different names*

### Comparing `unbeheader-1.0.2/unbeheader/headers.py` & `unbeheader-1.0.4/unbeheader/headers.py`

 * *Files identical despite different names*

### Comparing `unbeheader-1.0.2/unbeheader/util.py` & `unbeheader-1.0.4/unbeheader/util.py`

 * *Files identical despite different names*

### Comparing `unbeheader-1.0.2/PKG-INFO` & `unbeheader-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbeheader
-Version: 1.0.2
+Version: 1.0.4
 Summary: Never fail to maintain your file headers
 Home-page: https://github.com/unconventional/unbeheader
 License: MIT
 Author: Adrian Moennich
 Author-email: adrian.moennich@cern.ch
 Maintainer: Alejandro Avilés
 Maintainer-email: ome@unconventional.dev
@@ -64,33 +64,33 @@
 
 ### Usage
 
 It's possible to run Unbeheader in two modes: `fix` and `check`. The `fix` mode will update all files in the project with the correct header. The `check` mode will check that all files in the project have the correct header and exit with a non-zero status code if any file is missing or has an incorrect header.
 
 > **NOTE:** Neither `fix` or `check` modes will work unless Unbeheader can find a `.header.yaml` configuration file. Read more on the [Configuration](#configuration) section.
 
-To run Unbeheader in `fix` mode simply run the `unbeheader` command:
+To run Unbeheader in `fix` mode simply run the `unbehead` command:
 
 ```sh
-unbeheader                            # Update all the files in the Git repository
-unbeheader --path .                   # Update all the files under the current directory
-unbeheader --path /path/to/directory  # Update all the files under a directory
-unbeheader --path /path/to/file.py    # Update a single file
+unbehead                            # Update all the files in the Git repository
+unbehead --path .                   # Update all the files under the current directory
+unbehead --path /path/to/directory  # Update all the files under a directory
+unbehead --path /path/to/file.py    # Update a single file
 ```
 
 By default, Unbeheader will pass the current year to generate the `{dates}` placeholder in the header template. To pass a different year, use the `--year` flag:
 
 ```sh
-unbeheader --year 1947
+unbehead --year 1947
 ```
 
 To run Unbeheader in `check` mode, use the `--ci` flag:
 
 ```sh
-unbehader --ci
+unbehead --ci
 ```
 
 ## Configuration
 
 Unbeheader reads its configuration from `.header.yaml` files placed in the file tree of the project. It is possible to override configuration values by placing `.header.yaml` files in subdirectories. This is useful when different headers are needed for different parts of the project. It is also possible to exclude a directory by placing an empty `.no-header` file in it.
 
 Here is an example of a project structure with various `.header.yaml` and `.no-header` files:
@@ -121,15 +121,15 @@
 
 Setting value keys:
 - `root`: When set to `true`, it will stop Unbeheader from looking for `.header.yaml` files in parent directories. It defaults to `false`.
 - `substring`: The substring that Unbeheader will look for to determine if a file has a header or not. If the substring is not found, Unbeheader will assume that the file has no header. It defaults to `This file is part of`.
 
 Template value keys:
 - `owner`: The owner of the project, used to generate the `{owner}` placeholder. This key is required.
-- `start_year`: The start year of the header, used to generate the `{dates}` placeholder. It defaults to the year passed to the `unbeheader` command.
+- `start_year`: The start year of the header, used to generate the `{dates}` placeholder. It defaults to the year passed to the `unbehead` command.
 
 Finally, the `template` key is a multi-line string that will be used to generate the header template. The template accepts the interpolation of certain placeholders. These are:
 
 - `{comment_start}`: The comment start string for the file type (e.g. `#` for Python files).
 - `{comment_middle}`: The comment middle string for the file type (e.g. ` *` for CSS files).
 - `{comment_end}`: The comment end string for the file type (e.g. ` */` for CSS files).
 - `{dates}`: The start and end years of the header (e.g. `1904 - 1947`).
@@ -159,25 +159,25 @@
 
 You may now create the virtualenv and install the project with its dependencies in it with `poetry`:
 
 ```sh
 poetry install
 ```
 
-Once installed, you can invoke the `unbeheader` command with:
+Once installed, you can invoke the `unbehead` command with:
 
 ```sh
 poetry run -- unbeheader
 ```
 
 For convenience, you may want to spawn a shell within the virtualenv with:
 
 ```sh
 poetry shell
-unbeheader
+unbehead
 ```
 
 ### Contributing
 
 This project uses GitHub Actions to run the tests and linter on every pull request to the `master` and `devel` branches. You are still encouraged to run the tests and linter locally before pushing your changes.
 
 Tests can be run with:
```

