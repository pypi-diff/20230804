# Comparing `tmp/gpt-code-edit-1.0.1.tar.gz` & `tmp/gpt-code-edit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-code-edit-1.0.1.tar", last modified: Fri Aug  4 14:05:12 2023, max compression
+gzip compressed data, was "gpt-code-edit-1.0.2.tar", last modified: Fri Aug  4 14:16:59 2023, max compression
```

## Comparing `gpt-code-edit-1.0.1.tar` & `gpt-code-edit-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 14:05:12.122372 gpt-code-edit-1.0.1/
--rw-rw-rw-   0        0        0     5342 2023-08-04 14:05:12.120373 gpt-code-edit-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4526 2023-08-04 13:57:08.000000 gpt-code-edit-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 14:05:12.067371 gpt-code-edit-1.0.1/chatgpt_cli/
--rw-rw-rw-   0        0        0        0 2023-08-04 09:45:39.000000 gpt-code-edit-1.0.1/chatgpt_cli/__init__.py
--rw-rw-rw-   0        0        0     7541 2023-08-04 09:31:34.000000 gpt-code-edit-1.0.1/chatgpt_cli/arguement_validator.py
--rw-rw-rw-   0        0        0    11011 2023-07-19 16:18:28.000000 gpt-code-edit-1.0.1/chatgpt_cli/code_parser.py
--rw-rw-rw-   0        0        0     6467 2023-08-04 13:43:04.000000 gpt-code-edit-1.0.1/chatgpt_cli/gpt_request.py
--rw-rw-rw-   0        0        0     1061 2023-08-04 13:58:33.000000 gpt-code-edit-1.0.1/chatgpt_cli/main.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:05:12.118370 gpt-code-edit-1.0.1/gpt_code_edit.egg-info/
--rw-rw-rw-   0        0        0     5342 2023-08-04 14:05:11.000000 gpt-code-edit-1.0.1/gpt_code_edit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-08-04 14:05:11.000000 gpt-code-edit-1.0.1/gpt_code_edit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 14:05:11.000000 gpt-code-edit-1.0.1/gpt_code_edit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-08-04 14:05:11.000000 gpt-code-edit-1.0.1/gpt_code_edit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       66 2023-08-04 14:05:11.000000 gpt-code-edit-1.0.1/gpt_code_edit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-04 14:05:11.000000 gpt-code-edit-1.0.1/gpt_code_edit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 14:05:12.123371 gpt-code-edit-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1313 2023-08-04 14:04:56.000000 gpt-code-edit-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:16:59.174688 gpt-code-edit-1.0.2/
+-rw-rw-rw-   0        0        0     5492 2023-08-04 14:16:59.172671 gpt-code-edit-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4676 2023-08-04 14:13:07.000000 gpt-code-edit-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 14:16:59.102671 gpt-code-edit-1.0.2/chatgpt_cli/
+-rw-rw-rw-   0        0        0        0 2023-08-04 09:45:39.000000 gpt-code-edit-1.0.2/chatgpt_cli/__init__.py
+-rw-rw-rw-   0        0        0     7541 2023-08-04 09:31:34.000000 gpt-code-edit-1.0.2/chatgpt_cli/arguement_validator.py
+-rw-rw-rw-   0        0        0    11011 2023-07-19 16:18:28.000000 gpt-code-edit-1.0.2/chatgpt_cli/code_parser.py
+-rw-rw-rw-   0        0        0     6467 2023-08-04 13:43:04.000000 gpt-code-edit-1.0.2/chatgpt_cli/gpt_request.py
+-rw-rw-rw-   0        0        0     1061 2023-08-04 13:58:33.000000 gpt-code-edit-1.0.2/chatgpt_cli/main.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:16:59.166668 gpt-code-edit-1.0.2/gpt_code_edit.egg-info/
+-rw-rw-rw-   0        0        0     5492 2023-08-04 14:16:58.000000 gpt-code-edit-1.0.2/gpt_code_edit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-08-04 14:16:59.000000 gpt-code-edit-1.0.2/gpt_code_edit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 14:16:58.000000 gpt-code-edit-1.0.2/gpt_code_edit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-08-04 14:16:58.000000 gpt-code-edit-1.0.2/gpt_code_edit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       66 2023-08-04 14:16:58.000000 gpt-code-edit-1.0.2/gpt_code_edit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-04 14:16:58.000000 gpt-code-edit-1.0.2/gpt_code_edit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 14:16:59.175670 gpt-code-edit-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1313 2023-08-04 14:16:52.000000 gpt-code-edit-1.0.2/setup.py
```

### Comparing `gpt-code-edit-1.0.1/PKG-INFO` & `gpt-code-edit-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-code-edit
-Version: 1.0.1
+Version: 1.0.2
 Summary: A command line interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits including refactoring, adding comments, adding docstrings, or adding error handling.
 Home-page: https://github.com/ben-23-96/chatgpt_code_improve_cli
 Author: Ben Speakman
 Author-email: benspeakman23@yahoo.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -24,15 +24,15 @@
 - An active OpenAI account with API keys
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install My CLI.
 
 ```bash
-pip install chatgpt-cli
+pip install gpt-code-edit
 ```
 
 ## Usage
 
 ### Set API Key
 
 First, you need to set your OpenAI API key. You can find your key at [OpenAI Platform](https://platform.openai.com/account/api-keys) if you have a valid OpenAI account.
@@ -53,14 +53,16 @@
 
 ```bash
 gpt code-edit <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...] [--refactor] [--comments] [--docstrings] [--error-handling] [--gpt-4] [--temp <temperature>] [--create-review-file] [--edit-code-in-file]
 ```
 
 **Note**: One of `--create-review-file` or `--edit-code-in-file` must be set. Both can be set at the same time.
 
+**Note**: One of `--refactor`, `--comments`, `--docstrings` or `--error-handling` must be set. Multiple can be set at the same time.
+
 #### Arguments
 
 | Argument | Description |
 | :--- | :--- |
 | `<filename>` | The filename of the file containing the code (eg. main.py). |
 | `--target-functions` | A space-separated list of function names to be targeted. |
 | `--target-classes` | A space-separated list of class names to be targeted. Each class should be provided as `ClassName`. This will target every method in each class provided. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
@@ -68,15 +70,15 @@
 | `--refactor` | If set, refactor the code. |
 | `--comments` | If set, add comments to the code. |
 | `--docstrings` | If set, add docstrings to the code. |
 | `--error-handling` | If set, add error handling to the code. |
 | `--gpt-4` | If set, GPT-4 will be used instead of the default GPT-3. |
 | `--temp` | Affects the randomness of the output. A higher value makes the output more creative and a lower value makes it more structured. Must be between 1 and 0. The default is 0.4. |
 | `--create-review-file` | If set, creates a file `{function_name}.py` in a folder `gpt_edit_review` containing the newly edited function code and the old function code. This allows you to review the code before replacing it in the actual file. Remember to gitignore or delete the folder created when done. |
-| `--edit-code-in-file` | If set, rewrites the selected function with the newly edited version returned from GPT. If used, it is advisable for code to be committed and saved in case of erroneous changes. |
+| `--edit-code-in-file` | If set, rewrites the selected code within the file with the newly edited version returned from GPT. If used, it is advisable for code to be committed and saved in case of erroneous changes. |
 
 ### Review to File
 
 If when using code-edit the --create-review-file flag has been used so the edited code has been placed in a file for review, this command allows you to apply the changes to the actual file.
 
 ```bash
 gpt review-to-file <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...]
```

### Comparing `gpt-code-edit-1.0.1/README.md` & `gpt-code-edit-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 - An active OpenAI account with API keys
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install My CLI.
 
 ```bash
-pip install chatgpt-cli
+pip install gpt-code-edit
 ```
 
 ## Usage
 
 ### Set API Key
 
 First, you need to set your OpenAI API key. You can find your key at [OpenAI Platform](https://platform.openai.com/account/api-keys) if you have a valid OpenAI account.
@@ -37,14 +37,16 @@
 
 ```bash
 gpt code-edit <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...] [--refactor] [--comments] [--docstrings] [--error-handling] [--gpt-4] [--temp <temperature>] [--create-review-file] [--edit-code-in-file]
 ```
 
 **Note**: One of `--create-review-file` or `--edit-code-in-file` must be set. Both can be set at the same time.
 
+**Note**: One of `--refactor`, `--comments`, `--docstrings` or `--error-handling` must be set. Multiple can be set at the same time.
+
 #### Arguments
 
 | Argument | Description |
 | :--- | :--- |
 | `<filename>` | The filename of the file containing the code (eg. main.py). |
 | `--target-functions` | A space-separated list of function names to be targeted. |
 | `--target-classes` | A space-separated list of class names to be targeted. Each class should be provided as `ClassName`. This will target every method in each class provided. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
@@ -52,15 +54,15 @@
 | `--refactor` | If set, refactor the code. |
 | `--comments` | If set, add comments to the code. |
 | `--docstrings` | If set, add docstrings to the code. |
 | `--error-handling` | If set, add error handling to the code. |
 | `--gpt-4` | If set, GPT-4 will be used instead of the default GPT-3. |
 | `--temp` | Affects the randomness of the output. A higher value makes the output more creative and a lower value makes it more structured. Must be between 1 and 0. The default is 0.4. |
 | `--create-review-file` | If set, creates a file `{function_name}.py` in a folder `gpt_edit_review` containing the newly edited function code and the old function code. This allows you to review the code before replacing it in the actual file. Remember to gitignore or delete the folder created when done. |
-| `--edit-code-in-file` | If set, rewrites the selected function with the newly edited version returned from GPT. If used, it is advisable for code to be committed and saved in case of erroneous changes. |
+| `--edit-code-in-file` | If set, rewrites the selected code within the file with the newly edited version returned from GPT. If used, it is advisable for code to be committed and saved in case of erroneous changes. |
 
 ### Review to File
 
 If when using code-edit the --create-review-file flag has been used so the edited code has been placed in a file for review, this command allows you to apply the changes to the actual file.
 
 ```bash
 gpt review-to-file <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...]
```

### Comparing `gpt-code-edit-1.0.1/chatgpt_cli/arguement_validator.py` & `gpt-code-edit-1.0.2/chatgpt_cli/arguement_validator.py`

 * *Files identical despite different names*

### Comparing `gpt-code-edit-1.0.1/chatgpt_cli/code_parser.py` & `gpt-code-edit-1.0.2/chatgpt_cli/code_parser.py`

 * *Files identical despite different names*

### Comparing `gpt-code-edit-1.0.1/chatgpt_cli/gpt_request.py` & `gpt-code-edit-1.0.2/chatgpt_cli/gpt_request.py`

 * *Files identical despite different names*

### Comparing `gpt-code-edit-1.0.1/chatgpt_cli/main.py` & `gpt-code-edit-1.0.2/chatgpt_cli/main.py`

 * *Files identical despite different names*

### Comparing `gpt-code-edit-1.0.1/gpt_code_edit.egg-info/PKG-INFO` & `gpt-code-edit-1.0.2/gpt_code_edit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-code-edit
-Version: 1.0.1
+Version: 1.0.2
 Summary: A command line interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits including refactoring, adding comments, adding docstrings, or adding error handling.
 Home-page: https://github.com/ben-23-96/chatgpt_code_improve_cli
 Author: Ben Speakman
 Author-email: benspeakman23@yahoo.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -24,15 +24,15 @@
 - An active OpenAI account with API keys
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install My CLI.
 
 ```bash
-pip install chatgpt-cli
+pip install gpt-code-edit
 ```
 
 ## Usage
 
 ### Set API Key
 
 First, you need to set your OpenAI API key. You can find your key at [OpenAI Platform](https://platform.openai.com/account/api-keys) if you have a valid OpenAI account.
@@ -53,14 +53,16 @@
 
 ```bash
 gpt code-edit <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...] [--refactor] [--comments] [--docstrings] [--error-handling] [--gpt-4] [--temp <temperature>] [--create-review-file] [--edit-code-in-file]
 ```
 
 **Note**: One of `--create-review-file` or `--edit-code-in-file` must be set. Both can be set at the same time.
 
+**Note**: One of `--refactor`, `--comments`, `--docstrings` or `--error-handling` must be set. Multiple can be set at the same time.
+
 #### Arguments
 
 | Argument | Description |
 | :--- | :--- |
 | `<filename>` | The filename of the file containing the code (eg. main.py). |
 | `--target-functions` | A space-separated list of function names to be targeted. |
 | `--target-classes` | A space-separated list of class names to be targeted. Each class should be provided as `ClassName`. This will target every method in each class provided. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
@@ -68,15 +70,15 @@
 | `--refactor` | If set, refactor the code. |
 | `--comments` | If set, add comments to the code. |
 | `--docstrings` | If set, add docstrings to the code. |
 | `--error-handling` | If set, add error handling to the code. |
 | `--gpt-4` | If set, GPT-4 will be used instead of the default GPT-3. |
 | `--temp` | Affects the randomness of the output. A higher value makes the output more creative and a lower value makes it more structured. Must be between 1 and 0. The default is 0.4. |
 | `--create-review-file` | If set, creates a file `{function_name}.py` in a folder `gpt_edit_review` containing the newly edited function code and the old function code. This allows you to review the code before replacing it in the actual file. Remember to gitignore or delete the folder created when done. |
-| `--edit-code-in-file` | If set, rewrites the selected function with the newly edited version returned from GPT. If used, it is advisable for code to be committed and saved in case of erroneous changes. |
+| `--edit-code-in-file` | If set, rewrites the selected code within the file with the newly edited version returned from GPT. If used, it is advisable for code to be committed and saved in case of erroneous changes. |
 
 ### Review to File
 
 If when using code-edit the --create-review-file flag has been used so the edited code has been placed in a file for review, this command allows you to apply the changes to the actual file.
 
 ```bash
 gpt review-to-file <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...]
```

### Comparing `gpt-code-edit-1.0.1/setup.py` & `gpt-code-edit-1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="gpt-code-edit",
-    version="1.0.1",
+    version="1.0.2",
     packages=find_packages(),
 
     # Metadata
     author="Ben Speakman",
     author_email="benspeakman23@yahoo.com",
     description="A command line interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits including refactoring, adding comments, adding docstrings, or adding error handling.",
     long_description=open('README.md').read(),
```

